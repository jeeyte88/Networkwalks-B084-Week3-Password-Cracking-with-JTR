# Networkwalks-B084-Week3-Password-Cracking-with-JTR
Lab documentation for password cracking exercises (JTR + network tools) — methodology, results, and security recommendations.

# 🔐 W3-PM-Work | Cybersecurity NetworkWalks

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Program](https://img.shields.io/badge/Program-NetworkWalks-blue)
![Module](https://img.shields.io/badge/Module-Password%20Security-orange)

---


| 🏷️ Field | 📋 Details |
|---|---|
| 👤 **Pentester Name** | Abdikani Mohamud Jeite *(Cybersecurity Professional)* |
| 🎓 **Program / Batch** | B084-Networkwalks |
| 📅 **Date** | 18 November 2026 |
| ✅ **Modules Completed** | 🛠️ W2-PM1: Multiple Kali Tools <br> 🔍 W2-PM5: Zenmap Scanning |
| 🎯 **Client / Target** | 1️⃣ Password testing in a controlled lab environment using authorized files <br> 2️⃣ Password security testing using authorized lab exercises and tools |
| 🔓 **Permission Secured from Client?** | ✅ **Yes** |
| 📌 **Phases Covered** | 🔑 W3-PM1: Password Cracking with JTR <br> 🌐 W3-PM2: Password Cracking with NW Tools |

---

### 📂 About This Repository
> This repository documents authorized password security testing conducted as part of the **NetworkWalks Cybersecurity Program**, covering password hash cracking with John the Ripper and network-based credential testing tools — following ethical hacking standards in a fully controlled lab environment.

---

## 📖 Introduction

Password security remains one of the most fundamental — and most frequently exploited — aspects of information security. Despite advances in authentication technology, weak, reused, or poorly protected passwords continue to be a leading cause of unauthorized access across systems and networks. This module introduces participants to password cracking as a core skill in offensive security testing and defensive auditing, covering both the theory behind password storage and the practical tools used to evaluate password strength.

Over the course of this session, participants explore two complementary approaches: cracking passwords from captured hash files using dedicated tools like **John the Ripper**, and testing authentication mechanisms directly over network services using **network-based attack tools**. Together, these labs build a well-rounded understanding of how attackers target credentials — and, more importantly, how security professionals use the same techniques to strengthen defenses, enforce better password policies, and identify vulnerabilities before malicious actors can exploit them.

> ⚠️ **Ethical Notice:** All exercises in this report were carried out in a controlled, authorized lab environment only, reflecting standard ethical hacking practice. These techniques should never be applied to systems or accounts without explicit permission.

---
## 🔑 W3-PM1: Password Cracking with JTR

### 📄 File: My Locked PDF1

| 🏷️ Field | 📋 Details |
|---|---|
| 🎯 **Objective** | Recover the password protecting this PDF using John the Ripper (via the Johnny GUI) |
| 🛠️ **Tool Used** | Johnny (GUI for John the Ripper) |
| ⚙️ **Method** | 1️⃣ Extracted the password hash from the PDF using `pdf2john.pl`, producing a `$pdf$...` formatted hash <br> 2️⃣ Loaded the hash into Johnny <br> 3️⃣ Ran a dictionary/wordlist-based password-cracking attack against the hash |
| 🔢 **Hash Format** | `$pdf$4*4*128*-102...` (PDF format, as shown in the Hash/Formats columns) |
| ✅ **Result** | **Cracked** — password recovered: `good-luck` |
| 📊 **Status** | 100% (1/1 cracked, 0 left) |
| 🔍 **Observations** | Password was a simple dictionary word with a hyphen — easily guessed, indicating weak password policy on the source document. No complexity (no numbers, mixed case, or special character variation beyond the hyphen). |

#### 🖼️ Evidence / Screenshot

![Password Cracked](goodluck1.png)


![Password Cracked](enter pass1.png)

![Password Cracked](congrats1.png)

---


### 📄 File: My Locked PDF2

| 🏷️ Field | 📋 Details |
|---|---|
| 🎯 **Objective** | Recover the password protecting this PDF using John the Ripper (via the Johnny GUI) |
| 🛠️ **Tool Used** | Johnny (GUI for John the Ripper) |
| ⚙️ **Method** | 1️⃣ Extracted the password hash from the PDF via `pdf2john.pl`, producing a `$pdf$...` formatted hash <br> 2️⃣ Loaded the hash into Johnny <br> 3️⃣ Ran a dictionary-based password-cracking attack against the hash |
| 🔢 **Hash Format** | `$pdf$4*4*128*-102...` (PDF format) |
| ✅ **Result** | **Cracked** — password recovered: `password1` |
| 📊 **Status** | 100% (1/1 cracked, 0 left) |
| 🔍 **Observations** | An extremely common/weak password found near the top of most standard wordlists (e.g., `rockyou.txt`). One of the most frequently used passwords globally, demonstrating how trivial it is to crack when users don't follow password complexity guidelines. |

#### 🖼️ Screenshot



---













