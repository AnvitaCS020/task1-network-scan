# Task 1 - Network Port Scan

## Objective
Scan local network to discover open ports.

## Tool Used
Nmap 7.99

## Command Used
nmap -sS -T4 10.26.12.0/24

## Scan Results
| IP Address | Open Ports | Service |
|------------|-----------|---------|
| 10.26.12.223 | 53 | DNS - Router |
| 10.26.12.243 | None | Unknown Device |
| 10.26.12.177 | 135, 139, 445, 3306 | My PC |

## Security Risks Found
- Port 445 (SMB) - Vulnerable to WannaCry ransomware
- Port 3306 (MySQL) - Database exposed on network
- Port 135/139 (NetBIOS) - Legacy Windows services

## What I Learned
- How to perform a TCP SYN scan using Nmap
- How to identify open ports and services
- How to assess security risks from open ports
