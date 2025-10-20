
# Cyber Security Internship - Task 1

## Objective
To perform a local network port scan using Nmap and identify open ports and services.

## Tools Used
- Nmap
- Wireshark (optional)

## Steps Performed
1. Installed Nmap.
2. Found local IP range using `ipconfig`.
3. Ran TCP SYN scan with `nmap -sS 192.168.1.0/24`.
4. Saved scan results to `scan_results.txt`.
5. Identified open ports and their associated services.
6. Researched potential security risks.

## Output
- Open ports found: 22 (SSH), 80 (HTTP)
- Result file: `scan_results.txt`

## Learning Outcome
Gained understanding of port scanning, open ports, and network reconnaissance.
