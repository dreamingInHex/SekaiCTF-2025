
# 🏴 SekaiCTF 2025 — Prep & Question Bank

A **structured prep guide** for SekaiCTF 2025.  
Focus: **Know the questions before they’re asked.**  
Goal: **Be mentally and technically ready for any category.**

📅 **Event Date:** Aug 15–17, 2025 (48h online)  
🌐 [Official Site](https://ctf.sekai.team/) | [CTFTime Event Page](https://ctftime.org/event/2243/)

---

## 📂 Repository Layout

```plaintext
SekaiCTF-2025-Prep/
│
├── web/                         # Web Exploitation prep
│   └── README.md                 # Concepts, practice questions, resources
│
├── crypto/                      # Cryptography prep
│   └── README.md
│
├── pwn/                         # Binary Exploitation prep
│   └── README.md
│
├── rev/                         # Reverse Engineering prep
│   └── README.md
│
├── blockchain/                  # Smart Contracts & Blockchain prep
│   └── README.md
│
├── misc/                        # OSINT, Forensics, Stego, PPC prep
│   └── README.md
│
└── README.md                     # This file
````

---

## 🛠 General Prep Strategy

1. **Understand common challenge formats** for each category.
2. **Work through past SekaiCTF problems** — identify repeated patterns.
3. **Practice solving under time pressure** — speed matters as much as skill.
4. **Document solutions and methods** in the category READMEs for quick recall.

---

## 📜 Category Overview with Possible Questions & Prep Work

### 🕸 Web Exploitation

**Possible Questions:**

* Find & exploit an XSS in custom HTML/JS app
* SQL injection in a login or search form
* Bypass authentication using cookie manipulation
* SSRF to read local files or access internal services
* Exploit insecure deserialization in Node/PHP/Python
* Abuse weak JWT signing or key confusion
* Race condition in web request handling

**Prep Work:**

* Review: XSS payload crafting, SQLi techniques, SSRF bypasses
* Learn: Burp Suite basics, manual request crafting
* Practice: HackTheBox “Web” category, PortSwigger Web Academy

---

### 🔐 Cryptography

**Possible Questions:**

* Break RSA with small `e` or common modulus
* Recover key from reused nonce in ECDSA
* Decrypt CBC mode with padding oracle attack
* Frequency analysis for substitution ciphers
* Exploit poor PRNG seeding
* Lattice attacks on weak RSA parameters

**Prep Work:**

* Review: Modular arithmetic, number theory basics
* Learn: SageMath/Python crypto scripts
* Practice: Cryptopals challenges, PicoCTF crypto tasks

---

### 🖥 Pwn / Binary Exploitation

**Possible Questions:**

* Stack buffer overflow → ROP chain
* Format string vulnerability for info leak
* Heap exploitation (tcache poisoning, UAF)
* Bypassing NX, PIE, ASLR protections
* Shellcode injection

**Prep Work:**

* Review: C memory model, calling conventions
* Learn: Pwntools basics, GDB commands
* Practice: pwnable.kr, exploit.education

---

### 🔍 Reverse Engineering

**Possible Questions:**

* Crack password check in compiled binary
* Reverse a custom encryption algorithm
* Decode obfuscated logic in Python/Java
* Patch binary to bypass license check
* Analyze malware-like CTF binaries

**Prep Work:**

* Review: Assembly for x86/x64
* Learn: Ghidra or IDA Free navigation
* Practice: Crackmes.one, HTB “Reversing” challenges

---

### ⛓ Blockchain

**Possible Questions:**

* Exploit reentrancy in a smart contract
* Manipulate arithmetic to cause overflow/underflow
* Abuse delegatecall for takeover
* Steal funds via selfdestruct

**Prep Work:**

* Review: Solidity security patterns
* Learn: Foundry/Hardhat for local testing
* Practice: Ethernaut by OpenZeppelin

---

### 🧩 Misc / OSINT / Forensics

**Possible Questions:**

* Extract hidden data from images/audio
* Recover deleted files from disk image
* Find flags from social media clues
* Decode steganographic message
* Analyze packet capture for credentials

**Prep Work:**

* Review: `strings`, `binwalk`, `exiftool`, Wireshark basics
* Practice: CTFtime forensics/OSINT tasks, PicoCTF forensics

---

## 📚 Useful Resources

* **General:** [CTF Handbook](https://trailofbits.github.io/ctf/), [HackTricks](https://book.hacktricks.xyz/)
* **Web:** [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings)
* **Crypto:** [Cryptopals](https://cryptopals.com/)
* **Pwn:** [LiveOverflow YouTube](https://www.youtube.com/c/LiveOverflow)
* **Rev:** [Reverse Engineering for Beginners](https://beginners.re/)
* **Blockchain:** [Ethernaut](https://ethernaut.openzeppelin.com/)

---

**🎯 Mindset for SekaiCTF:**

> “You don’t need every tool — you need every *idea*.”

```

