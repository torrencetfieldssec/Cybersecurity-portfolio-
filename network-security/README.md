# Network Security
This file contains simulated network traffic labs I conducted utilizing tcpdump, Suricata and Wireshark.

## Packet Capture Explanation

Captured and analyzed live network traffic using `tcpdump` on a Linux VM to understand packet structures and network interface activity. This lab focused on filtering traffic on the `eth0` interface and inspecting packet details such as source, destination, protocol, and flags. 

---

### First Packet Capture
Demonstrates capturing the first few packets from the `eth0` interface and inspecting key packet data.

![First Packet Capture](screenshots/ns-first-packet.PNG)

---

### Detailed Packet Capture
This image shows a more detailed view of subsequent packets, including TCP flags, sequence numbers, and acknowledgment info.

![Detailed Packet Capture](screenshots/ns-first-packet2.PNG)
## Suricata Network Monitoring Explaination 

Suricata is an open source network threat detection engine that functions as an IDS/IPS and network security monitoring tool. It inspects network traffic in real time, detecting suspicious patterns, anomalies, and known threats using rules and signatures. The images below shows me using Suricata to monitor and analyze network packets for security events.

---

### Suricata Packet Capture 1
The image below shows the initial network traffic captured by Suricata.

![Suricata Capture 1](screenshots/ns-suricata1.PNG)

---

### Suricata Packet Capture 2
In this image I examined alerts, logs and other important information captured with Suricata.

![Suricata Capture 2](screenshots/ns-suricata2.PNG)


## Wireshark TCP Packet Capture

Wireshark is network protocol analyzer that allows you to capture and inspect live network traffic in detail. This example below focuses on TCP traffic, showing how connections are established and packets are exchanged between hosts. This application helps visualize network flows and troubleshoot or investigate potential security incidents.

---

### Wireshark TCP Capture
In this image I used Wireshark to analyze the contents of a packet that I captured for an security invesitagation that invloved a SYN attack on an fictional organization.

![Wireshark TCP Capture](screenshots/ns-wireshark-TCP.PNG)
## Skills Demonstrated

Network traffic capture and analysis  
Packet inspection and protocol understanding  
Intrusion detection and monitoring  
Security alert review and investigation  
Troubleshooting   

## Use Cases

Network monitoring and threat detection  
Incident investigation support  
Protocol and traffic analysis  
IDS/IPS usage
Security audits and compliance checks


