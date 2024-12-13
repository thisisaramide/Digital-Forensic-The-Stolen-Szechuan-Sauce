# Digital Forensics Investigation: The Stolen Szechuan Sauce

## Overview
This repository contains the findings and analysis from a digital forensics investigation conducted on a simulated cyber incident involving the theft of proprietary data. The investigation focused on identifying malicious activity, tracing the attacker's steps, and uncovering key evidence.

## Key Objectives
1. Identify malicious processes and their behavior.
2. Trace the source of the malware and its network communication.
3. Investigate data exfiltration activities, including the theft of sensitive files.
4. Reconstruct the timeline of events leading up to and during the attack.
5. Recommend architecture changes to enhance network security.

## Artifacts Analyzed
- **Memory Dump**: Used for process analysis and malware detection.
- **Disk Image**: Examined for file system anomalies, logs, and deleted files.
- **Network Capture (PCAP)**: Analyzed for suspicious IPs, payload delivery, and data exfiltration.
- **Autorun**: Investigated for persistence mechanisms and service configurations.

## Tools Used
- **Wireshark**: For network traffic analysis and artifact extraction.
- **Volatility**: For memory analysis (e.g., `pstree`, `malfind`, and `netscan` plugins).
- **Registry Explorer**: To investigate loaded hives and services.
- **VirusTotal**: For malware identification and validation.
- **Autopsy**: For disk image analysis and timeline reconstruction.
- **Ewftools**: For mounting the image.
- **Log2timeline**: For creating supertimeline.
- **Regripper**: For forensic artifacts with the use of plugins.
- **Registry Editor**: For manual viewing and editing of Windows Registry settings and configurations.

## Investigation Questions
1. What process was malicious?  
2. Identify the IP Address that delivered the payload.  
3. What IP Address is the malware calling to?  
4. Where is this malware on disk?  
5. When did it first appear?  
6. Did someone move it?  
7. What were the capabilities of this malware?  
8. Is this malware easily obtained?  
9. Was this malware installed with persistence on any machine?  
10. What malicious IP Addresses were involved?  
11. Did the attacker access any other systems?  
12. Did the attacker steal or access any data?  
13. What was the network layout of the victim network?  
14. What architecture changes should be made immediately?  
15. Did the attacker steal the Szechuan sauce? If so, what time?  
16. Did the attacker steal or access any other sensitive files? If so, what times?  

## Recommendations
- Restrict remote desktop access to internal connections only and enforce VPN use for remote access.
- Implement multi-factor authentication (MFA) to secure login mechanisms.
- Regularly monitor logs and network traffic for brute-forcing or anomalous activity.
- Conduct regular vulnerability assessments to mitigate entry-point exploitation.
