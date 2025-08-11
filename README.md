```markdown
# 🏴 SekaiCTF 2025 Preparation & Exploitation Toolkit

A comprehensive collection of **tools**, **guides**, **automation scripts**, and **cheat sheets** to assist with challenges in [SekaiCTF 2025](https://ctf.sekai.team/)  
(Aug 15–17, 2025 — Online).

This repository is built for **pre-event preparation** and **rapid in-event exploitation**, designed to speed up common tasks such as reconnaissance, analysis, and exploitation for all major CTF categories.

---

## 📅 Event Overview

**Name:** SekaiCTF 2025  
**Dates:** Aug 15–17, 2025 (48 hours, Online)  
**Format:** Jeopardy-style (points-based, multiple independent challenges)  
**Difficulty:** Beginner → Advanced  
**Special Note:** Dual pre-qualifier for:
- **10th XCTF Finals (2026) — China**
- **MaltaCTF Finals (2025) — Malta**

### Expected Challenge Categories
From past years (and the 2025 announcements), we expect:

- **Web Exploitation** — XSS, SQLi, SSRF, race conditions, CSP bypass, server misconfigs
- **Cryptography** — Classical, modern, applied crypto attacks (RSA, ECC, hash collisions)
- **Pwn / Binary Exploitation** — Buffer overflows, heap exploitation, ret2libc, Windows kernel
- **Reverse Engineering** — Crackmes, obfuscated binaries, reversing protocols
- **Miscellaneous / OSINT** — Steganography, forensics, open-source intelligence
- **Programming / PPC** — Algorithmic problems, data parsing, automation
- **Blockchain** — Solidity/Web3 exploitation, smart contract bugs (reentrancy, delegatecall, signature forgery)

⚠ **Prize Bounty Alert** — 2025 includes **four blockchain challenges with USDT bounties** for the fastest solves.

---

## 📂 Repository Layout

The repository is structured for **speed** and **clarity** during the event:

```

SekaiCTF-2025-Toolkit/
│
├── tools/                      # Pre-built tools & binaries
│   ├── crypto/                  # Crypto analysis helpers
│   ├── web/                     # Web exploitation utilities
│   ├── pwn/                     # Exploit frameworks/templates
│   ├── rev/                     # Reverse engineering tools
│   └── blockchain/              # Smart contract & Web3 exploitation
│
├── guides/                     # Markdown-based knowledge base
│   ├── web.md                   # Web exploitation tactics
│   ├── crypto.md                # Crypto attacks and formulas
│   ├── pwn.md                   # Binary exploitation techniques
│   ├── reverse-engineering.md   # Static/dynamic reversing workflows
│   ├── blockchain.md            # Ethereum/Solidity exploitation
│   └── misc.md                  # Forensics, OSINT, stego
│
├── scripts/                    # Ready-to-run scripts
│   ├── recon/                   # Enumeration & fingerprinting
│   ├── exploitation/            # Payload generators, PoCs
│   └── analysis/                 # Parsers, format analyzers
│
├── writeups/                   # Store event notes and solutions
└── README.md                   # This file

````

---

## 🛠 Recommended Local Environment

Before the CTF begins, **set up a clean, reproducible environment**.

### Base OS / Environment
- Ubuntu 22.04 LTS (or WSL2)
- Python 3.11+ with `pipenv` or `virtualenv`
- Docker & Docker Compose
- Node.js 18+ (for blockchain/web tasks)

### Core Packages
**Install globally (or in a dedicated VM/container):**
```bash
sudo apt update && sudo apt install -y \
    git build-essential python3 python3-pip python3-venv \
    gdb binwalk exiftool jq netcat nmap socat \
    curl wget unzip xxd file
````

**Python packages:**

```bash
pip install pwntools requests flask beautifulsoup4 pycryptodome
```

---

## 🔍 Category-specific Tool Recommendations

### Web Exploitation

* `Burp Suite` / `ZAP`
* `ffuf`, `gobuster` — Directory brute-forcing
* `sqlmap` — SQL injection automation
* `nuclei` — Vulnerability scanning templates

### Cryptography

* `sagemath`
* `RsaCtfTool`
* `hashcat`, `john` — Password/hash cracking
* `xortool` — XOR key recovery

### Binary Exploitation / Reverse Engineering

* `pwntools` — Exploit scripting
* `gdb` with `gef` or `peda`
* `radare2` / `cutter`
* `ghidra` / `Binary Ninja` (if licensed)

### Blockchain

* `foundry` (`forge`, `cast`) — Smart contract development/testing
* `hardhat` — Ethereum dev environment
* `slither` — Static analysis
* `ethers.js` / `web3.py` — Interaction scripts

### Misc / Forensics

* `binwalk`, `foremost`, `strings`
* `steghide`, `zsteg` — Steganography
* `volatility3` — Memory forensics

---

## 📖 Guide Philosophy

Each `guides/*.md` file contains:

* **Quick reference** — Commands, payloads, formulas
* **Step-by-step exploitation patterns**
* **Past SekaiCTF-specific quirks** — Lessons from previous years
* **Links to deeper reading** — Docs, blog posts, whitepapers

Example in `guides/web.md`:

```markdown
## XSS Quick Payloads
- Basic: `<script>alert(1)</script>`
- Event handler: `<img src=x onerror=alert(1)>`
- Polyglot: `"><svg onload=confirm(1)>`
...
```

---

## ⚡ Quick Start Workflow

1. **Clone & prepare**:

```bash
git clone https://github.com/<your-username>/SekaiCTF-2025-Toolkit.git
cd SekaiCTF-2025-Toolkit
```

2. **Install dependencies**:

```bash
pip install -r requirements.txt
```

3. **Recon target quickly**:

```bash
python scripts/recon/dirbust.py http://target.ctf/
```

4. **Exploit / test**:

```bash
python scripts/exploitation/pwn_template.py target-ip 31337
```

5. **Log progress in `writeups/`**.

---

## 📌 CTF Day Tips

* **Speed > Perfection** — Solve what you can quickly, leave harder challenges for later.
* **Take notes in real-time** — Even messy notes can be cleaned later for writeups.
* **Watch the scoreboard** — Track which categories are bleeding points.
* **Monitor Discord** — Sometimes clarifications or hints drop there.

---

## 📚 Useful References

* [SekaiCTF Official](https://ctf.sekai.team/)
* [CTFTime — SekaiCTF 2024](https://ctftime.org/event/2243/tasks/)
* [HackTricks](https://book.hacktricks.xyz/)
* [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings)
* [Awesome CTF](https://github.com/apsdehal/awesome-ctf)

---

**Happy hacking & good luck!** 🐾
*“Preparation wins before the first packet is sent.”*
