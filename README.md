
# Cyber Security Internship - Task 1

## Objective
To perform a local network port scan using Nmap and identify open ports and services.

## Tools Used
- Nmap
- Wireshark (optional)

## Steps Performed
1. Installed Nmap.
2. Found local IP range using `ipconfig`.
3. Ran TCP SYN scan with `nmap -sS 192.168.1.0/24`. # this is example
4. Saved scan results to `scan_results.txt`.
5. Identified open ports and their associated services.
6. Researched potential security risks.

## Output
- Open ports found: 135/tcp  open  msrpc,  
                    139/tcp  open  netbios-ssn, 
                    445/tcp  open  microsoft-ds, 
                    7070/tcp
- Result file: `scan_results.txt`

## Common Services and Risks Identified 

| Port | Service | Risk | Action |
|------|----------|------|--------|
| 22 | SSH | Possible brute-force attacks | Use SSH key authentication |
| 80 | HTTP | Unencrypted web traffic | Enable HTTPS |
| 445 | SMB | Vulnerable to ransomware | Disable SMB if not required |
| 3389 | RDP | Remote login attacks | Use strong passwords or disable if unused |

## ⚙️ All Nmap Commands Used

Below are all the practical Nmap commands used to perform the port scanning task and related analysis.

---

### 🔹 1. Check Nmap Installation
```bash
nmap --version
ipconfig
nmap -sn 192.168...../24  #Discover Active Devices (Ping Scan)
nmap -sS 192.168.56.0/24  #Basic TCP SYN Scan (Stealth Scan)
nmap -sS 192.168.56.0/24 -oN "%userprofile%\Documents\scan_results.txt"  #Save Scan Output to a File



## Summary
From the scan, I learned that open ports can reveal critical services to attackers. 
Securing or closing unused ports reduces the attack surface and improves overall network security.

## Learning Outcome
Gained understanding of port scanning, open ports, and network reconnaissance.
