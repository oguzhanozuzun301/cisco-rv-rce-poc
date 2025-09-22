# CVE-2023-20048 — Cisco RV Series PoC & Exploit

**⚠ WARNING:** For **authorized testing only**. Do not use against systems you do not own or have written permission to test. This is a **Proof of Concept** for **authorized testing only**.  

## What this is
Small repository with:
- `CiscoPoc.py` — harmless PoC to check for CVE-2023-20048.
- `CiscoRCE.py` — exploit that attempts a reverse shell via the vulnerable `form2ping.cgi`.
- 
## **Description**  
This script checks if a **Cisco RV Series router** is vulnerable to **CVE-2023-20048**, a command injection flaw leading to **RCE as root**.  

## Requirements
- Python 3.8+
- `requests` (`pip install requests`)

## Usage

### Check (PoC)
```bash
python3 CiscoPoc.py -t <TARGET_IP> -u <USER> -p <PASS>
