# Task 1: Basic Network Scanning with Nmap

##  Objective
The primary goal of this task is to perform an active reconnaissance on a target system to identify open ports, active services, and the operating system details. This is the first step in a security assessment to map the attack surface of a network.

##  Tools Used
* **Nmap (Network Mapper):** A powerful command-line tool used for network discovery and security auditing.
* **Zenmap:** The official Nmap Security Scanner GUI, used for visualizing network topology and results.

##  Steps Performed
1. **Target Selection:** Identified an authorized target for scanning (`scanme.nmap.org`).
2. **Scan Configuration:** Utilized the **Intense Scan** profile in Zenmap, which executes the command: `nmap -T4 -A -v`.
   - `-T4`: Set the timing template for faster execution.
   - `-A`: Enables OS detection, version detection, script scanning, and traceroute.
   - `-v`: Increases verbosity to show real-time progress.
3. **Execution:** Ran the scan to probe the target's ports and services.
4. **Analysis:** Inspected the **Ports/Hosts** tab to analyze service versions and the **Topology** tab to visualize the network path.
5. **Security Assessment:** Evaluated the risks associated with open ports (e.g., HTTP on Port 80, SSH on Port 22).

##  Outcome & Findings
- **Open Ports Identified:** Discovered services such as HTTP (Port 80) and Nping-echo (Port 9929).
- **Service Versioning:** Identified the specific versions of software running, allowing for vulnerability cross-referencing.
- **Firewall Detection:** Observed "Filtered" states on several ports, indicating the presence of a firewall or packet filtering system.
- **Topology:** Successfully mapped the network hops from the local machine to the remote target.



---
*Completed as part of the Oasis Infobyte Security Analyst Internship.*
