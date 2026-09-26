# networkwalks-B083E-Week3

# 🔐 Week 3 — Password Cracking

<div align="center">

# Cybersecurity & Ethical Hacking

### Password Cracking with John the Ripper, Johnny GUI & Networkwalks Tools

**WEEK 3 | PROJECT MODULE 1 & 2**

</div>

---

## 📌 Overview

This week's cybersecurity lab focused on understanding the fundamentals of **password cracking** and password cracking in a controlled ethical-hacking environment.

The lab consisted of two tasks:

1. **Password Cracking with John the Ripper (JTR) and Johnny**
2. **Password Cracking with Networkwalks Hash Calculator and Password Cracker**

In both exercises, the objective was to crack the password of a provided password-protected PDF file.

The exercises demonstrated the basic password-cracking workflow:

```text
Protected PDF
     ↓
Extract PDF Password Hash
     ↓
Provide Hash to Cracking Tool
     ↓
Password cracking
     ↓
Use cracked Password
     ↓
Open Protected PDF
```

> ⚠️ **Ethical & Legal Notice:**
> These techniques were performed only against the password-protected PDF provided for this authorized cybersecurity training lab. Password-cracking techniques should only be used on systems, files, or credentials that you own or have explicit permission to test.

---

# 🎯 Objectives

The main objectives of this week's lab were:

* Understand the concept of password cracking.
* Understand how protected files store password-related information.
* Extract a password hash from a protected PDF.
* Use **John the Ripper** to perform password cracking.
* Use **Johnny**, the graphical interface for John the Ripper.
* Use the **Networkwalks Hash Calculator**.
* Use the **Networkwalks Password Cracker**.
* Compare a local password-cracking workflow with a browser-based workflow.
* Understand why weak passwords can be cracked relatively easily.

---

# 🧰 Tools & Technologies

| Tool                              | Purpose                                       |
| --------------------------------- | --------------------------------------------- |
| **John the Ripper (JTR)**         | Password/hash cracking                        |
| **Johnny GUI**                    | Graphical interface for John the Ripper       |
| **Networkwalks Hash Calculator**  | Extract password hash from protected PDF      |
| **Networkwalks Password Cracker** | Attempt password cracking from extracted hash |
| **Windows PC**                    | Primary lab environment                       |
| **Web Browser**                   | Access Networkwalks online tools              |
| **Notepad**                       | Save extracted hash for JTR                   |

---

# 📁 Lab File

The lab used the following password-protected PDF:

```text
My Locked PDF1.pdf
My Locked PDF2.pdf
```

The PDF was provided as part of the authorized Networkwalks cybersecurity training exercise.

---

# 🔹 TASK 1 — Password Cracking with John the Ripper

## 1. Download John the Ripper

The first task involved installing **John the Ripper** on the Windows system.

John the Ripper is a password-security auditing and password-cracking tool capable of working with multiple password hash formats.



---

## 2. Install / Configure Johnny

**Johnny** provides a graphical interface for John the Ripper, making it easier to perform password-cracking operations without relying entirely on the command line.

After installing Johnny, the application was opened and its settings were configured to use the John executable.


---

## 3. Configure John.exe

Inside Johnny's settings, the John executable was selected.

The `john.exe` file was located inside the **run** directory of the John the Ripper installation.


---

## 4. Obtain the Protected PDF

The provided encrypted PDF was downloaded to the Windows system.

```text
My Locked PDF1.pdf
```


---

## 5. Extract the PDF Hash

The PDF password hash was extracted using a PDF hash extraction tool.

The extracted value used the PDF hash format beginning with:

```text
$pdf$4*4*128*-1028*1*16*34eb542eff4e1b0b32d25ce15a9a7281*32*b77872bfc9a24fb2f845066283a8fc1b0021446990b9e4114071a4d9104984c1*32*e7572256e4b552cd57988f5134214b91920d94d7a6bf550ea94a2995c7f2ab02
```

The complete hash was copied for use with John the Ripper.

### Screenshot — Extracted Hash

> `<img width="1103" height="387" alt="image" src="https://github.com/user-attachments/assets/01b0c448-5743-47a1-818b-02f5884ce21f" />
`

> **Important:** The complete hash must be copied without accidentally removing any part of the value.

---

## 6. Save the Hash

A text file was created using Notepad to store the extracted PDF hash.

The file was saved as:

```text
hash1.txt
```

The hash was stored in the text file in the format required by John the Ripper.

### Screenshot — Hash in Notepad

> 📸 **Screenshot Placeholder:**
> `![Hash in Notepad](screenshots/task1/08-hash-notepad.png)`

### Screenshot — Saving hash1.txt

> 📸 **Screenshot Placeholder:**
> `![Saving Hash File](screenshots/task1/09-save-hash-file.png)`

---

## 7. Open Hash File in Johnny

Johnny was opened again and the saved hash file was loaded using the **Open Password File** option.

### Screenshot — Open Password File

> 📸 **Screenshot Placeholder:**
> `![Open Password File](screenshots/task1/10-open-password-file.png)`

---

## 8. Start Password Attack

After loading the hash file, a new password-cracking attack was started.

Johnny then used John the Ripper to attempt to crack the password represented by the PDF hash.

### Screenshot — Starting Attack

> 📸 **Screenshot Placeholder:**
> `![Start New Attack](screenshots/task1/11-start-attack.png)`

---

## 9. Password cracked

The password was successfully cracked by the cracking process.

### Screenshot — cracked Password

> 📸 **Screenshot Placeholder:**
> `![cracked Password](screenshots/task1/12-cracked-password.png)`

The cracked password was:

```text
password1
```

---

## 10. Verify the Password

The cracked password was entered into the protected PDF.

### Screenshot — Entering cracked Password

> 📸 **Screenshot Placeholder:**
> `![Enter PDF Password](screenshots/task1/13-enter-password.png)`

The PDF opened successfully after entering the cracked password.

### Screenshot — Successfully Opened PDF

> 📸 **Screenshot Placeholder:**
> `![Opened PDF](screenshots/task1/14-opened-pdf.png)`

### ✅ Task 1 Result

The password-protected PDF was successfully opened after cracking its password using **John the Ripper / Johnny**.

---

# 🔹 TASK 2 — Password Cracking with Networkwalks Tools

The second task demonstrated a browser-based password-cracking workflow using Networkwalks tools.

This workflow consisted of:

```text
Protected PDF
     ↓
Networkwalks Hash Calculator
     ↓
PDF Hash
     ↓
Networkwalks Password Cracker
     ↓
cracked Password
     ↓
Open PDF
```

---

## 1. Download the Protected PDF

The same lab PDF was obtained from the Networkwalks project task page.

```text
My Locked PDF1.pdf
```

### Screenshot — Downloaded PDF

> 📸 **Screenshot Placeholder:**
> `![Networkwalks PDF](screenshots/task2/01-locked-pdf.png)`

---

## 2. Open Networkwalks Hash Calculator

The **Networkwalks Hash Calculator** was opened in a web browser.

The tool was used to extract the password hash from the protected PDF.

### Screenshot — Hash Calculator

> 📸 **Screenshot Placeholder:**
> `![Hash Calculator](screenshots/task2/02-hash-calculator.png)`

---

## 3. Upload the PDF

The protected PDF was uploaded to the Hash Calculator.

### Screenshot — Uploading PDF

> 📸 **Screenshot Placeholder:**
> `![Upload PDF](screenshots/task2/03-upload-pdf.png)`

---

## 4. Extract the Hash

After processing the PDF, the Hash Calculator displayed the PDF password hash.

The hash started with:

```text
$pdf$
```

### Screenshot — Generated PDF Hash

> 📸 **Screenshot Placeholder:**
> `![Generated Hash](screenshots/task2/04-generated-hash.png)`

The complete hash was copied for the next stage.

---

## 5. Open Networkwalks Password Cracker

The **Networkwalks Password Cracker** was opened in the browser.

### Screenshot — Password Cracker

> 📸 **Screenshot Placeholder:**
> `![Password Cracker](screenshots/task2/05-password-cracker.png)`

---

## 6. Submit the Hash

The extracted PDF hash was pasted into the Password Cracker.

### Screenshot — Hash Submitted

> 📸 **Screenshot Placeholder:**
> `![Hash Submitted](screenshots/task2/06-hash-submitted.png)`

---

## 7. Start the Cracking Process

The password-cracking process was started.

The tool attempted different password candidates until the correct password was identified.

### Screenshot — Cracking Process

> 📸 **Screenshot Placeholder:**
> `![Cracking Process](screenshots/task2/07-cracking-process.png)`

---

## 8. Password cracked

The password was successfully cracked.

### Screenshot — Cracked Password

> 📸 **Screenshot Placeholder:**
> `![Cracked Password](screenshots/task2/08-cracked-password.png)`

The cracked password was:

```text
password1
```

---

## 9. Verify Password Against PDF

The cracked password was entered into the protected PDF.

### Screenshot — Enter Password

> 📸 **Screenshot Placeholder:**
> `![Enter Password](screenshots/task2/09-enter-password.png)`

The PDF opened successfully.

### Screenshot — Successfully Opened PDF

> 📸 **Screenshot Placeholder:**
> `![Opened PDF](screenshots/task2/10-opened-pdf.png)`

### ✅ Task 2 Result

The password-protected PDF was successfully opened after cracking its password using the **Networkwalks Hash Calculator** and **Password Cracker**.

---

# 🔬 Technical Understanding

## What is Password Cracking?

Password cracking is the process of attempting to crack a password from a protected system, file, or stored password representation.

In a controlled security assessment, password cracking can help determine whether passwords are sufficiently resistant to guessing and automated attacks.

---

## What is a Hash?

A hash is a value generated from input data using a hashing algorithm.

In password-security systems, hashes can be used to represent passwords without storing the original password directly.

For this lab, the protected PDF contained information that could be converted into a PDF password hash compatible with password-cracking tools.

The extracted value had the general format:

```text
$pdf$...
```

---

## How the Lab Worked

The overall process can be represented as:

```text
                 PASSWORD-PROTECTED PDF
                           │
                           ▼
                  Extract PDF Hash
                           │
                           ▼
                      $pdf$...
                           │
              ┌────────────┴────────────┐
              │                         │
              ▼                         ▼
      John the Ripper            Networkwalks
          / Johnny              Password Cracker
              │                         │
              ▼                         ▼
        Password cracking       Password cracking
              │                         │
              └────────────┬────────────┘
                           ▼
                    cracked Password
                           │
                           ▼
                  Open Protected PDF
```

---

# 📊 Task Comparison

| Feature               | Task 1                   | Task 2                        |
| --------------------- | ------------------------ | ----------------------------- |
| Environment           | Windows                  | Windows / Browser             |
| Hash Extraction       | PDF hash extraction tool | Networkwalks Hash Calculator  |
| Cracking Tool         | John the Ripper / Johnny | Networkwalks Password Cracker |
| Installation Required | Yes                      | No                            |
| Interface             | Desktop GUI              | Web-based                     |
| Input                 | PDF hash file            | PDF hash                      |
| Result                | cracked password       | cracked password            |
| PDF Verification      | ✅ Successful             | ✅ Successful                  |

---

# 🧠 Key Learning Outcomes

Through these exercises, I learned:

### 1. Passwords can be tested through their protected representations

A protected file does not necessarily need to expose the original password for a password-cracking attack to be attempted.

### 2. Hash extraction is an important step

Before a cracking tool can attempt password cracking, the relevant password hash or encrypted-file representation needs to be obtained in a format the tool understands.

### 3. Password complexity affects cracking difficulty

Simple and predictable passwords can potentially be cracked much faster than long, unique passwords.

### 4. Different tools can perform similar security testing tasks

The first task demonstrated a local desktop-based workflow using John the Ripper and Johnny, while the second demonstrated a browser-based workflow.

### 5. Password security is important

The lab demonstrates why users and organizations should avoid short, predictable, and commonly used passwords.

---

# 🛡️ Security Recommendations

Based on the lab results, the following password-security practices are recommended:

* Use long and unique passwords.
* Avoid common words and predictable patterns.
* Avoid reusing passwords across multiple services.
* Use a reputable password manager.
* Enable multi-factor authentication where available.
* Use strong password policies for organizational systems.
* Regularly test password security in authorized environments.
* Never attempt to crack passwords belonging to systems or files without authorization.

---

# 📸 Evidence

Screenshots documenting the completed lab are organized into the following directories:

```text
screenshots/
│
├── task1/
│   ├── 01-john-download.png
│   ├── 02-johnny-installation.png
│   ├── 03-johnny-interface.png
│   ├── 04-select-john-exe.png
│   ├── 05-locked-pdf.png
│   ├── 06-pdf-upload.png
│   ├── 07-pdf-hash.png
│   ├── 08-hash-notepad.png
│   ├── 09-save-hash-file.png
│   ├── 10-open-password-file.png
│   ├── 11-start-attack.png
│   ├── 12-cracked-password.png
│   ├── 13-enter-password.png
│   └── 14-opened-pdf.png
│
└── task2/
    ├── 01-locked-pdf.png
    ├── 02-hash-calculator.png
    ├── 03-upload-pdf.png
    ├── 04-generated-hash.png
    ├── 05-password-cracker.png
    ├── 06-hash-submitted.png
    ├── 07-cracking-process.png
    ├── 08-cracked-password.png
    ├── 09-enter-password.png
    └── 10-opened-pdf.png
```

---

# ✅ Final Results

| Task                 | Activity                                         | Result       |
| -------------------- | ------------------------------------------------ | ------------ |
| **Task 1**           | Password cracking using John the Ripper / Johnny | ✅ Completed  |
| **Task 2**           | Password cracking using Networkwalks tools       | ✅ Completed  |
| **PDF Verification** | Open protected PDF using cracked password      | ✅ Successful |

Both Week 3 password-cracking exercises were successfully completed in the authorized cybersecurity training environment.

---

# 🎓 Conclusion

Week 3 provided practical exposure to password-cracking concepts and demonstrated the complete workflow from **protected file → hash extraction → password cracking → password verification**.

The exercises also highlighted an important cybersecurity principle: **password strength directly affects resistance to password-cracking attacks**.

The lab was performed strictly for educational and authorized cybersecurity training purposes.

---

## 📚 References

* John the Ripper — Openwall
* Johnny — Graphical interface for John the Ripper
* Networkwalks — Cybersecurity & Ethical Hacking Project Tasks

---

<div align="center">

### 🔐 Cybersecurity & Ethical Hacking — Week 3

**Password Cracking Lab**

</div>
