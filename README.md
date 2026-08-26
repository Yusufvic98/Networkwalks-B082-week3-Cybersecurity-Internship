# Networkwalks-B082-week3-Cybersecurity-Internship
PASSWORD CRACKING AT JOHNNY REAPER &amp; NETWORKWALKS WEBSITE
## 🔐 Week Three — Password Cracking & PDF Password Recovery

**Networkwalks Academy Cybersecurity Internship | Ethical Hacking Track**

> ⚠️ **Disclaimer:** All activities in this project were performed exclusively on training files supplied by Networkwalks Academy, within an authorized laboratory environment. No unauthorized systems, accounts, or files were accessed. This repository is for educational and portfolio purposes only.

---

### 📋 Overview

This project documents my Week Three practical exercise for the Networkwalks Academy cybersecurity internship, focused on **password cracking and password recovery for encrypted PDF documents**. The goal was to understand how security professionals test password strength using offline hash-based recovery techniques, and to apply that knowledge through two independent toolchains — one local, one browser-based.

The full write-up, including step-by-step methodology and screenshot evidence, is available here:
📄 **[Networkwalks_Week3_Password_Cracking_Report.pdf](./Networkwalks_Week3_Password_Cracking_Report.pdf)**

---

### 🎯 Objectives

- Understand the concept and purpose of password cracking
- Distinguish between an encrypted file and a crackable hash representation
- Install and configure **John the Ripper (Jumbo)** and the **Johnny GUI** on Windows
- Extract a PDF-compatible hash from a password-protected document
- Perform a controlled, offline password-recovery attack
- Use **Networkwalks'** browser-based hash extraction and cracking laboratory
- Validate recovered passwords by successfully opening the original protected files
- Document findings and defensive security recommendations

---

### 🧰 Tools & Technologies

| Tool | Purpose |
|---|---|
| **John the Ripper (Jumbo)** | Offline password-hash cracking engine |
| **Johnny** | Graphical front-end for John the Ripper |
| **pdf2john-based hash extractor** | Converts an encrypted PDF into a crackable `$pdf$` hash |
| **Networkwalks Hash Calculator** | Browser-based PDF hash extraction |
| **Networkwalks Password Cracker** | Browser-based candidate testing engine |

---

### 🧪 Module Summary

| Module | Toolchain | Target | Recovered Password | Flag |
|---|---|---|---|---|
| **Module One** | John the Ripper + Johnny (local) | Locked PDF 3 | `1qaz2wsx` | `nw{networkwalks_flag_260821_1}` |
| **Module Two** | Networkwalks Hash Calculator + Password Cracker (web) | Locked PDF 2 | `password1` | `nw{networkwalks_persistence_jtr_270521}` |

**Workflow (both modules):**
```
Encrypted PDF → Hash extraction ($pdf$) → Password-candidate testing → Recovered password → Validation
```

---

### 🔍 Key Findings

- Weak, predictable, or keyboard-pattern passwords (`1qaz2wsx`, `password1`) can be recovered quickly through offline attacks.
- Password **length, uniqueness, and unpredictability** are far more important defensive factors than the mere presence of a password.
- Offline cracking means an attacker doesn't need repeated access to the original file once a hash is obtained — protecting hashes and encrypted backups matters as much as protecting the passwords themselves.
- A tool reporting a "successful crack" should always be validated by actually opening the original protected file.

---

### 🛡️ Defensive Recommendations

- Use long, unique, unpredictable passwords — avoid keyboard patterns and common words
- Adopt a password manager for generation and secure storage
- Enable multi-factor authentication wherever supported
- Treat extracted hashes and cracking artifacts as sensitive data
- Conduct periodic, authorized password-strength audits

---

### 🧠 Skills Gained

`Password Security` · `John the Ripper` · `Johnny GUI` · `PDF Hash Extraction` · `Dictionary Attacks` · `Web-Based Password Auditing` · `Evidence Documentation` · `Ethical Hacking Methodology` · `Cybersecurity Reporting`

---

### 📁 Repository Contents

```
├── Networkwalks_Week3_Password_Cracking_Report.pdf   # Full detailed report with evidence screenshots
└── README.md                                          # This summary
```

---

### 👤 Author

**Oyewumi Yusuf Olayemi**
Cybersecurity Intern — Networkwalks Academy
Tutor: Waqas Karim
📧 Yusufvic98@gmail.com
