# Task 8: Network Traffic Capture and Analysis

## Objective
To capture live network traffic and analyze HTTP packets to understand how data is transmitted over an unencrypted connection.

## Tool Used
- **Wireshark:** A network protocol analyzer used for troubleshooting and security analysis.

## Methodology
1. Captured traffic on the active network interface.
2. Filtered the capture for `http` protocol packets.
3. Analyzed the GET requests and responses to view headers and payload data.

## Findings
By analyzing the HTTP packets, I was able to see plain-text data including:
- **Host:** The destination server address.
- **User-Agent:** Information about the browser used.
- **Accept-Language:** The language settings of the client.

**Security Observation:** Since the data is sent via HTTP (Port 80) and not HTTPS (Port 443), an attacker on the same network could perform a "Sniffing" attack to read this sensitive information.
