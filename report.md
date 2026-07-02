Network Traffic Analysis Report
1. Objective

The objective of this project was to capture and analyze real-time network traffic generated from everyday web browsing using Wireshark. The goal was to understand how different network protocols operate during normal internet usage.

2. Tools Used
Wireshark (Network Protocol Analyzer)
Windows Operating System
Google Chrome Browser

3. Methodology
Installed Wireshark and Npcap on Windows.
Started packet capture on the active Wi-Fi interface.
Visited multiple public websites such as Wikipedia, Python.org, StackOverflow, and OpenAI.
Captured network traffic for approximately 2–3 minutes.
Saved the capture file in .pcapng format for analysis.

4. Protocols Observed
DNS (Domain Name System)
Used to resolve domain names into IP addresses.
Visible queries for websites like wikipedia.org, python.org, etc.
TCP (Transmission Control Protocol)
Establishes reliable communication using a three-way handshake (SYN, SYN-ACK, ACK).
TLS (Transport Layer Security)
Used for encrypted HTTPS communication.
Packet contents appear as “Application Data” or “Ciphertext”.
HTTPS
Secure web communication protocol.
Ensures encryption of user data.

5. Key Observations
Most modern web traffic is encrypted using TLS.
No readable application data was visible due to HTTPS encryption.
DNS requests revealed visited domains.
TCP ensured reliable packet delivery.
Multiple secure connections were established to CDN and cloud servers.

6. Conclusion
The analysis shows that modern internet communication relies heavily on encryption (HTTPS/TLS), ensuring privacy and security. While packet contents are not visible, metadata such as DNS queries, IP addresses, and protocol behavior can still be analyzed effectively using Wireshark.