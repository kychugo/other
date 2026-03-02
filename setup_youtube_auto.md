要由零開始建立呢個自動化平台，我會將成個過程拆解成 **5 個階段**。請跟住下面嘅步驟一步步嚟，因為只要其中一個 API 冇整好，成套嘢就郁唔到。

---

### 第一階段：安裝系統工具（最重要）

呢個專案唔單止係 Python，佢仲依賴兩個好重要嘅外部軟件：

1.  **安裝 Python**: 去 [python.org](https://www.python.org/) 下載並安裝最新版（記得剔 **"Add Python to PATH"**）。
2.  **安裝 FFMPEG**:
    *   去 [ffmpeg.org](https://ffmpeg.org/download.html) 下載。
    *   解壓後，將 `bin` 資料夾嘅路徑加到你電腦嘅 **「系統環境變數 (PATH)」** 注入。
    *   *測試方法*：喺 CMD 打 `ffmpeg -version`，見到版本號就成功。
3.  **安裝 ImageMagick (MoviePy 必須)**:
    *   去 [ImageMagick 下載頁](https://imagemagick.org/script/download.php#windows)。
    *   **重要**：安裝時一定要剔 **"Install legacy utilities (e.g. convert)"**。
    *   安裝完後，搵到 `magick.exe` 嘅路徑。

---

### 第二階段：準備 Python 環境

1.  喺你電腦開個新 Folder（例如 `YoutubeAuto`），將所有 Source Code 擺入去。
2.  打開 Terminal / CMD，進入呢個 Folder，執行：
    ```bash
    pip install -r requirements.txt
    ```
3.  **設定 ImageMagick 路徑** (Windows 用家常犯錯誤)：
    *   搵到你 Python 庫入面 `moviepy/config_defaults.py` 呢個檔案。
    *   將 `IMAGEMAGICK_BINARY` 改成你安裝 ImageMagick 嘅路徑，例如：
        `IMAGEMAGICK_BINARY = r"C:\Program Files\ImageMagick-7.1.1-Q16-HDRI\magick.exe"`

---

### 第三階段：申請 API 權限（拎「通行證」）

#### 1. Reddit API (拎資料)
*   去 [Reddit App Preferences](https://www.reddit.com/prefs/apps)。
*   撳 "Create another app"，揀 **"script"**。
*   Name 隨便寫，Redirect URI 寫 `http://localhost:8080`。
*   你就會得到 **Client ID** (喺名稱下面嗰串字) 同 **Secret Key**。
*   **建立 `secrets.txt`**: 喺根目錄建立呢個檔案，內容格式：
    ```text
    你的ClientID,你的SecretKey
    你的Reddit用戶名,你的Reddit密碼
    ```

#### 2. YouTube API (自動上傳)
*   去 [Google Cloud Console](https://console.cloud.google.com/)。
*   建立新專案，喺 Library 搜尋並 **Enable "YouTube Data API v3"**。
*   去 "OAuth consent screen" 設定為 "External"，求其填資料。
*   去 "Credentials" -> "Create Credentials" -> **"OAuth client ID"**。
*   Application type 揀 **"Desktop app"**。
*   下載 JSON 檔案，改名做 **`client_secret.json`**，擺喺專案根目錄。

---

### 第四階段：準備素材 (Assets)

Code 入面引用咗好多圖同片，你要預備好：
1.  **建立資料夾結構**:
    *   `assets/backgrounds/`: 擺一個 `minecraft_background.mp4` (或者你自己鍾意嘅背景片)。
    *   `assets/reddit/`: 擺 Reddit 嘅 icon，例如 `r_askreddit_dark.png`、`title_topbar_dark.png` 等圖（你要跟返 Code 入面嘅檔名搵圖或自己執圖）。
    *   `assets/transitions/`: 擺 `no_signal.mp4` 做轉場。
    *   建立空白嘅 `audio/` 同 `output/` 資料夾。

---

### 第五階段：正式執行

#### 1. 生成影片
執行 `main.py`。
```bash
python main.py
```
*   **發生咩事？**：程式會去 AskReddit 爬文 -> 用 TikTok API 攞聲 -> 用 MoviePy 剪片 -> 產出 `.mp4` 擺喺 `output/`。
*   **檢查**：去 `output/` 睇吓條片成唔成功，字體同聲啱唔啱。

#### 2. 上傳影片
執行 `upload.py`。
```bash
python upload.py
```
*   **發生咩事？**：第一次行會彈個網頁出嚟叫你 Google Login。登入完，個 Script 就會自動幫你上傳 `output/` 裡面嘅片。

---

### 疑難排解 (Common Issues)
*   **TikTok 聲攞唔到？**: 檢查網絡，或者可能係 TikTok 暫時封咗嗰個 API Endpoint。
*   **MoviePy 報錯 `ImageMagick`？**: 100% 係因為你冇喺 `config_defaults.py` 設定啱個 `magick.exe` 路徑。
*   **YouTube 上傳唔到？**: 檢查你個 `client_secret.json` 係咪擺啱位。注意 YouTube API 每日有上傳配額（通常每日可以上傳約 5-6 條片）。

如果你跟住呢套流程做，你就有咗一套**全自動化嘅 YouTube 賺錢機器**！有邊一步卡住咗可以再問我。
