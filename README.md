# 🔐 Week 3: Password Cracking Lab

> Part of my Cyber Security journey with **NetworkWalks**

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Topic](https://img.shields.io/badge/Topic-Password%20Cracking-blue)
![Environment](https://img.shields.io/badge/Environment-Lab%20Only-orange)

---

## 📌 Objective

To understand how password hashes work and how weak passwords can be recovered using **dictionary attacks**, and to learn why strong password practices matter.

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **John the Ripper (Johnny GUI)** | Running a dictionary attack on a PDF hash |
| **NetworkWalks Hash Calculator** | Extracting a crackable `$pdf$` hash from a password-protected PDF |
| **NetworkWalks Password Cracker** | Cracking the extracted hash with a wordlist |

---

## 📚 Modules Completed

### ✅ W3-PM1: Password Cracking with John the Ripper (JtR)
1. Took a password-protected PDF provided in the lab
2. Extracted its hash
3. Loaded the hash into **Johnny** (the JtR GUI)
4. Ran a **dictionary attack** using a wordlist
5. Password recovered and the PDF unlocked

### ✅ W3-PM2: Password Cracking with NW Tools
1. Uploaded the locked PDF into the **NW Hash Calculator** (parsed locally)
2. Extracted the `$pdf$` hash (pdf2john / hashcat compatible format)
3. Pasted the hash into the **NW Password Cracker**
4. Ran the attack using a wordlist
5. Password cracked successfully, PDF opened and the flag was captured 🚩

---

## 🔄 Workflow

```
Locked PDF  →  Extract Hash  →  Dictionary Attack  →  Password Found  →  PDF Unlocked  →  Flag Captured
```

---

## 💡 Key Learnings

- Passwords are protected by **hashes**, and weak passwords can still be cracked
- **Dictionary attacks** are very fast against common or predictable passwords
- Real password strength = **length + complexity + uniqueness**
- Understanding how attackers think is the first step to **defending better**

---

## 🛡️ Defense Tips

- Use **long passphrases** instead of short, common words
- Never reuse passwords across accounts
- Use a **password manager**
- Enable **MFA** everywhere possible

---

## ⚠️ Disclaimer

This work was done in a **controlled lab environment** for **educational purposes only**. Do not attempt password cracking on systems or files you do not own or have explicit permission to test.

---
