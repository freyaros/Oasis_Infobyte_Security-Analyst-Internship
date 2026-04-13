# Task 1: Network Scanning with Nmap/Zenmap

## Scan Results Summary
- **Target:** scanme.nmap.org
- **Scan Type:** Intense Scan (-T4 -A -v)

## Port State Analysis
| Color in Zenmap | State | Meaning |
| :--- | :--- | :--- |
| **Green** | Open | A service is actively listening (e.g., HTTP/HTTPS). |
| **Red** | Closed | No service is listening, but the host is reachable. |
| **Yellow/Gray** | Filtered | A firewall is blocking the scan probes. |

## Significance
Identifying open ports allows us to check for outdated service versions that might have known vulnerabilities. Filtered ports indicate a healthy defense-in-depth strategy using firewalls.
