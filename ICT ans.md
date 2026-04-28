This model answer provides the correct options for the multiple-choice questions from the 2026-DSE-ICT exam paper, along with a detailed reasoning for each answer.

---

### **2026-DSE-ICT Model Answers**

#### **Question 1**
**Original Question:** Which of the following is **not** an example of data verification for an online shop?
*   A. A customer enters a password twice during the creation of an account.
*   B. Two staff members enter the same set of data into a database independently.
*   C. A staff member checks another staff member's input data against the original data.
*   D. A computer program checks the input dates against calendar rules.

**Model Answer:** **D**
**Reasoning:** Verification is the process of checking data for accuracy by comparing it to a source or through redundant entry (Options A, B, and C). Option D describes **data validation**, which is checking if the data is sensible or follows specific rules (like range or format checks).

---

#### **Question 2**
**Original Question:** Which of the following is/are the advantage(s) of using Unicode over ASCII?
(1) Unicode includes more language characters, such as Japanese characters.
(2) Unicode requires less storage space than ASCII.
(3) Unicode includes the symbols '@' and '&'.
*   A. (1) only
*   B. (2) only
*   C. (1) and (3) only
*   D. (2) and (3) only

**Model Answer:** **A**
**Reasoning:** Unicode was designed to support thousands of characters from all global languages (1), whereas ASCII is limited to 128 characters. Unicode generally requires **more** storage space (e.g., 16-bit or 32-bit vs ASCII's 7/8-bit) (2). Symbols like '@' and '&' are already present in standard ASCII (3).

---

#### **Question 3**
**Original Question:** Compared to H.264, H.265 is a better video compression standard for MP4. Which of the following statements is correct?
*   A. H.264 does not support video streaming.
*   B. With H.265, the file size is generally smaller.
*   C. H.265 is better because it is an open source codec.
*   D. A GPU is necessary for using H.265.

**Model Answer:** **B**
**Reasoning:** H.265 (HEVC) offers much better compression efficiency than H.264, meaning it can maintain the same video quality at roughly half the bitrate, resulting in smaller file sizes.

---

#### **Question 4**
**Original Question:** A computer system uses 20 bits to store each user number, where the last bit is a parity bit. How many user numbers can the system support?
*   A. $19^2$
*   B. $20^2$
*   C. $2^{19}$
*   D. $2^{20}$

**Model Answer:** **C**
**Reasoning:** Out of 20 bits, 1 bit is reserved for parity, leaving 19 bits for actual data (the user number). The number of unique combinations for 19 bits is $2^{19}$.

---

#### **Question 5**
**Original Question:** Which of the following 8-bit numbers using two's complement representation, when multiplied by -1, will cause an overflow error?
*   A. 1000 0000
*   B. 1111 1111
*   C. 0000 0000
*   D. 0111 1111

**Model Answer:** **A**
**Reasoning:** The range for 8-bit two's complement is -128 to 127. `1000 0000` represents -128. If multiplied by -1, the result is +128, which exceeds the maximum representable positive value (127), thus causing an overflow.

---

#### **Question 6**
**Original Question:** [Refer to Spreadsheet] The formula in C2 is copied to C3:C5 to find the rank... highest points will be ranked as 1. What is the formula in C2?
*   A. `=RANK(B2, $B$2:$B$5, 0)`
*   B. `=RANK(B2, B$2:B$5, 2)`
*   C. `=RANK(B2, $B2:$B5, 0)`
*   D. `=RANK(B2, $B2:$B5, 2)`

**Model Answer:** **A**
**Reasoning:** To rank from highest to lowest, the 'order' argument in the RANK function should be 0 (or omitted). To ensure the range remains the same when the formula is copied down, absolute cell references (`$B$2:$B$5`) must be used.

---

#### **Question 7**
**Original Question:** [Refer to Pivot Table] What is the summary function?
*   A. Product
*   B. Sum
*   C. Maximum
*   D. Average

**Model Answer:** **D**
**Reasoning:** The pivot table shows decimal values (like 3.8). Functions like Sum, Max, and Product on integers (ratings 1-5) would result in whole numbers. Average is the only function likely to produce these decimal results from a set of ratings.

---

#### **Question 8**
**Original Question:** A company builds its web site with a new design and information architecture. Which of the following processes are involved?
(1) Data analysis, (2) Data organisation, (3) Data presentation
*   A. (1) and (2) only
*   B. (1) and (3) only
*   C. (2) and (3) only
*   D. (1), (2) and (3)

**Model Answer:** **D**
**Reasoning:** Information architecture involves understanding user needs (Analysis), structuring how content is categorized and linked (Organisation), and determining how that structure is displayed to the user (Presentation).

---

#### **Question 9**
**Original Question:** [Refer to SQL and Table MEM] How many records will be output?
*   A. 0 | B. 1 | C. 2 | D. 3

**Model Answer:** **B**
**Reasoning:**
1. `WHERE CAT LIKE 'M%'` filters records: M1001 (Award M1111, Pts 2), M1211 (Award M1247, Pts 1), M1111 (Award M2330, Pts 5), M1331 (Award M1111, Pts 2).
2. `GROUP BY AWARD`:
   - M1111: Sum(2+2) = 4
   - M1247: Sum(1) = 1
   - M2330: Sum(5) = 5
3. `HAVING SUM(POINT) > 4`: Only group M2330 (Sum=5) satisfies this.
Result: 1 record.

---

#### **Question 10**
**Original Question:** Which of the following is the main purpose of using data control in information processing?
*   A. To simplify the processing...
*   B. To ensure the data integrity.
*   C. To remove dependence on data security.
*   D. To enhance the efficiency of data compression.

**Model Answer:** **B**
**Reasoning:** Data control mechanisms (like validation, verification, and access controls) are primarily implemented to ensure that data remains accurate, consistent, and reliable (integrity).

---

#### **Question 11**
**Original Question:** A computer consists of a CPU and a GPU. Which of the following statements... is most appropriate?
*   A. Both have multiple cores that can execute instructions.
*   B. Both are optimised mainly for rendering graphics.
*   C. Both are always used together for executing tasks in data analysis together.
*   D. The CPU is used for multitasking, while the GPU is used for single-tasking.

**Model Answer:** **A**
**Reasoning:** While CPUs have a few complex cores for general multitasking and GPUs have thousands of simpler cores for parallel processing, both architectures utilize multiple cores to execute instructions.

---

#### **Question 12**
**Original Question:** Which of the following statements about the fetch-decode-execute cycle is/are correct?
(1) A program instruction is translated into machine code for program execution.
(2) A program instruction is divided into several parts for different CPU components to handle.
(3) Registers in a CPU are used to control the operations of processors.
*   A. (1) only | B. (2) only | C. (1) and (3) only | D. (2) and (3) only

**Model Answer:** **D**
**Reasoning:** Statement (1) describes compilation, which happens before the cycle begins. During the cycle, the instruction is already machine code. (2) is correct as the Decode stage splits the instruction into opcode and operands. (3) is correct as registers (like the Program Counter and Instruction Register) manage the cycle.

---

#### **Question 13**
**Original Question:** Which of the following best describes a parallel processing system?
*   C. It processes different tasks of a program at the same time.

**Model Answer:** **C**
**Reasoning:** Parallel processing is the simultaneous execution of multiple tasks (or parts of a task) using multiple processors or cores.

---

#### **Question 14**
**Original Question:** Batch processing is suitable for...
*   D. Student examination mark calculation

**Model Answer:** **D**
**Reasoning:** Batch processing is ideal for high-volume tasks that do not require immediate user interaction and can be processed all at once (e.g., end-of-semester calculations).

---

#### **Question 15**
**Original Question:** Before installing a major upgrade to the operating system... what should you do first?
*   B. Create a backup of important files on the computer.

**Model Answer:** **B**
**Reasoning:** Major upgrades carry a risk of data loss or system failure; having a backup is the most critical safety step.

---

#### **Question 16**
**Original Question:** Which of the following components in the glasses stores the system boot-up programs?
*   D. ROM

**Model Answer:** **D**
**Reasoning:** Read-Only Memory (ROM) is non-volatile and used to store firmware/BIOS needed to start the hardware and load the operating system.

---

#### **Question 17**
**Original Question:** Which of the following best describe the functions of a switch?
(1) Prevents data collisions during data transmission.
(2) It directs data to devices based on their MAC addresses.
(3) It directly connects a LAN to a WAN.
*   A. (1) and (2) only

**Model Answer:** **A**
**Reasoning:** Switches use MAC addresses to route data within a LAN and create separate collision domains to prevent collisions. Connecting a LAN to a WAN (Internet) is the job of a **router**.

---

#### **Question 18**
**Original Question:** A mobile device connects to a Wi-Fi network, but the connection speed is slow. Possible reason?
*   D. There are many concurrent users on the network.

**Model Answer:** **D**
**Reasoning:** Wi-Fi is a shared medium. As more users connect and transmit data simultaneously, the available bandwidth for each user decreases due to congestion and overhead.

---

#### **Question 19**
**Original Question:** Susan uses Bluetooth instead of Wi-Fi... Which of the following is a possible reason?
*   C. Bluetooth has lower power consumption.

**Model Answer:** **C**
**Reasoning:** Bluetooth is specifically designed for low-power, short-range communication, making it ideal for battery-operated peripherals.

---

#### **Question 20**
**Original Question:** Which of the following communication protocols is involved [in dividing data into packets]?
*   C. TCP

**Model Answer:** **C**
**Reasoning:** In the TCP/IP stack, the Transport Control Protocol (TCP) is responsible for breaking large data streams into smaller segments for transmission.

---

#### **Question 21**
**Original Question:** Function of a firewall?
*   D. Preventing network connections from unauthorised access.

**Model Answer:** **D**
**Reasoning:** A firewall acts as a barrier, monitoring and filtering incoming/outgoing traffic based on security rules to prevent unauthorized entry into a network.

---

#### **Question 22**
**Original Question:** Which of the following actions would likely be considered unethical?
(1) Student uses someone's program segment... without acknowledgment.
(3) A company removes digital watermarks from images... and posts them...
*   C. (1) and (3) only

**Model Answer:** **C**
**Reasoning:** Plagiarism (1) and removing watermarks to bypass copyright (3) are clear ethical violations. Monitoring employee browsing (2) is generally considered a standard business security practice, even if controversial.

---

#### **Question 23**
**Original Question:** [Refer to Article on employee bribes] What should the company have done to avoid this?
*   B. (2) only (Monitoring access to customers' data in real time)

**Model Answer:** **B**
**Reasoning:** Real-time monitoring can detect unauthorized or suspicious data access patterns by employees, helping to prevent internal data breaches.

---

#### **Question 24**
**Original Question:** Which of the following statements are correct?
(1) Installation of spyware enables unauthorised monitoring...
(2) Phishing can be conducted across numerous channels...
*   A. (1) and (2) only

**Model Answer:** **A**
**Reasoning:** Statement (3) is false because opening spam can lead to severe security risks like malware infections or identity theft, not just "annoyance."

---

#### **Question 25**
**Original Question:** Main purpose of using SSL?
*   D. To encrypt data transmitted via the Internet.

**Model Answer:** **D**
**Reasoning:** Secure Sockets Layer (SSL) is primarily used to secure sensitive data (like payment info) by encrypting the communication between the user's browser and the web server.

---

#### **Question 26**
**Original Question:** [Refer to Boolean Expressions with $X=-3, Y=1, Z=4$] Which returns **false**?
*   C. `(X + Y < -2 and Y - X = Z) and (X > Z)`

**Model Answer:** **C**
**Reasoning:** Substituting values: `(-3 + 1 < -2)` is `(-2 < -2)` which is **False**. In an `AND` operation, if any part is False, the whole expression is False.

---

#### **Question 27**
**Original Question:** [Refer to Algorithm with $X=6, Y=13$] What is the output?
*   A. 1

**Model Answer:** **A**
**Reasoning:**
- Pass 1: $Y = 13-3=10, X = 10-6=4$
- Pass 2: $Y = 10-3=7, X = 7-4=3$
- Pass 3: $Y = 7-3=4, X = 4-3=1$
- Pass 4: $Y = 4-3=1, X = 1-1=0$
The loop terminates because $X=0$ is not $\ge 1$. Output $Y = 1$.

---

#### **Question 28**
**Original Question:** [Refer to Array ch: A, B, C, D, E, F] Which value(s) in ch is/are 'K' after execution?
*   A. (1) only (`ch[1]`)

**Model Answer:** **A**
**Reasoning:** The loop shifts elements left. When $i=1$, `ch[1]` becomes `ch[2]` (which is 'C'). The `if` condition `ch[1] == 'C'` becomes True, and `ch[1]` is assigned 'K'. No other 'C' exists to trigger another assignment.

---

#### **Question 29**
**Original Question:** Which set of input data is most suitable for testing the algorithm?
*   D. 95 90 80 70 60 50

**Model Answer:** **D**
**Reasoning:** Option D includes values that test all ranges (above 90, between 70-90, below 70) and specifically includes the boundary values 90 and 70 to check the "greater than" logic.

---

#### **Question 30**
**Original Question:** What is the value of sum?
*   C. 28

**Model Answer:** **C**
**Reasoning:** Initially $N = [0, 1, 2... 10]$. The first loop changes elements $N[0]$ to $N[8]$ into the difference between their next two neighbors. Since the original values are consecutive integers ($i+2$ and $i+1$), the difference is always 1.
New array: $[1, 1, 1, 1, 1, 1, 1, 1, 1, 9, 10]$.
Sum = $9 \times 1 + 9 + 10 = 28$.

---

#### **Question 31**
**Original Question:** How many different values of $X$ can the algorithm generate?
*   B. 2

**Model Answer:** **B**
**Reasoning:**
- Sub-branch $X=10$ is impossible because if $P \ge Q$, it's logically impossible for $R > P$ and $Q > R$ to be true simultaneously.
- Sub-branch $X=30$ is impossible because if $P < Q$, $P$ cannot equal $Q$.
Only $X=20$ and $X=40$ can be reached.

---

#### **Question 32**
**Original Question:** What are the missing parts in Version 2?
*   D. (1) `k <- 10`, (2) `k <= 20`

**Model Answer:** **D**
**Reasoning:** To replicate a `for` loop from 10 to 20, the counter must start at 10 and continue running as long as it is less than or equal to 20.

---

#### **Question 33**
**Original Question:** How many '$' will be output?
*   C. 4

**Model Answer:** **C**
**Reasoning:** The loop runs while $x > 20$ and $y < 20$.
Pairs $(x, y)$: (40, 10) $\rightarrow$ Output 1; (35, 11) $\rightarrow$ Output 2; (30, 12) $\rightarrow$ Output 3; (25, 13) $\rightarrow$ Output 4.
Next is (20, 14). Since $x$ is not $> 20$, the loop stops.

---

#### **Question 34**
**Original Question:** Which statement X would cause an infinite loop?
*   A. (1) only (`s <- s + 6`)

**Model Answer:** **A**
**Reasoning:** Starting at $s=3$ and adding 6 gives: 3, 9, 15, 21, 27, 33, 39, 45, 51... It skips exactly 48, so the condition `s <> 48` remains True forever. Options (2) and (3) both reach 48.

---

#### **Question 35**
**Original Question:** What is the value of $n$?
*   A. -1

**Model Answer:** **A**
**Reasoning:** The last time the `if` triggers is when $i=9$. $n$ becomes 9. The while loop `n > 0` subtracts 2 repeatedly: 9, 7, 5, 3, 1, -1. At -1, the while loop stops. No other code changes $n$ after $i=9$.

---

#### **Question 36**
**Original Question:** What is the value of $a$?
*   C. 6

**Model Answer:** **C**
**Reasoning:** This is the Euclidean algorithm for GCD.
1. $a=48, b=18 \rightarrow temp=18, b=48\%18=12, a=18$
2. $a=18, b=12 \rightarrow temp=12, b=18\%12=6, a=12$
3. $a=12, b=6 \rightarrow temp=6, b=12\%6=0, a=6$
Loop ends when $b=0$. $a=6$.

---

#### **Question 37**
**Original Question:** Which is correct?
*   B. Line 3 has a logical error.

**Model Answer:** **B**
**Reasoning:** Line 3 says `while w <= 0 and h <= 0`. This only forces a re-entry if **both** are invalid. If a user enters a valid weight but an invalid height, the program would proceed with bad data. It should use `or`.

---

#### **Question 38**
**Original Question:** Which is correct?
*   B. Line 7 has a logical error.

**Model Answer:** **B**
**Reasoning:** The formula $bmi = w / h * h$ calculates $(w/h) \times h = w$ due to operator precedence. It should be $w / (h * h)$.

---

#### **Question 39**
**Original Question:** Which is correct?
*   D. There should be a digital certificate for a trusted HTTPS connection.

**Model Answer:** **D**
**Reasoning:** HTTPS relies on SSL/TLS certificates issued by a Trusted Certificate Authority (CA) to authenticate the website's identity to the user.

---

#### **Question 40**
**Original Question:** Peter develops open source software. Which is/are correct?
*   B. (2) only (Peter can sell the copies of the software.)

**Model Answer:** **B**
**Reasoning:** Open source licenses do not forbid commercial distribution. However, (1) is false because open source relies on copyright law to enforce its licenses, and (3) is false as the primary freedom of open source is that anyone can modify the code without seeking explicit permission.