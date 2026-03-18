# HawkEye Lab Final Report  
**Internship:** Nullclass Cybersecurity Internship  
**Intern:** Ismayeel khan 
**Date:** 12 Sept 2025  

---

## 1. Introduction  
This report covers the **HawkEye Lab** from CyberDefenders.  
I analyzed the provided PCAP file with Wireshark to investigate a HawkEye keylogger incident, identify IOCs, and track exfiltration of stolen data.  

---

## 2. Tools Used  
- Wireshark (packet analysis)  
- CyberChef (decoding)  
- Hashing tools (`certutil`)  
- CyberDefenders platform  
- VirusTotal

---

## 3. Steps Taken  
1. Opened the `stealer.pcap` file in Wireshark.  
2. Reviewed capture properties (packets, duration, timestamps).  
3. Checked active endpoints and traffic patterns.  
4. Exported HTTP objects → found malicious file download.  
5. Extracted and hashed the file.  
6. Traced SMTP traffic → found stolen data exfiltration.  
7. Decoded SMTP credentials to identify attacker details.  
8. Answered all 24 challenge questions and submitted successfully.  

---

## 4. Key Findings 
- Malicious file name: **tkraw_Protected99.exe**  
- The duration of the capture: **01:03:41**
- MD5 hash: **71826ba081e303866ce2a2534491a2f7** 
- Most active computer at the link: **00:08:02:1c:47:ae*
- Victim public IP: **173.66.146.112**  
- Email account used for exfiltration: **sales.del@macwinlogistics.in**  
- Malware variant: **HawkEye Stealer**  

---

## 5. Proof of Work  
- Screenshot: Wireshark analysis 1: https://github.com/IsmayeelKhan77/internship-projects/blob/main/wireshark-ss-1.png?raw=true
- Screenshot: Wireshark analysis 2: https://github.com/IsmayeelKhan77/internship-projects/blob/main/wireshark-ss-2.png?raw=true  
- Screenshot: Lab completion certificate:  https://github.com/IsmayeelKhan77/internship-projects/blob/main/hawkeye-intern-project.png?raw=true

---

## 6. Conclusion  
This lab gave me hands-on experience in:  
- Investigating real-world malware traffic.  
- Identifying IOCs like malicious files, hashes, and IPs.  
- Understanding data exfiltration via SMTP.  

✅ Completed all 24/24 questions.  
This was my **first full project** in the Nullclass internship.  

---

## Deliverables  
- `CyberDefender_Hawkeye` (this report)  
- 2 supporting screenshots  
- CyberDefenders badge link: https://cyberdefenders.org/blueteam-ctf-challenges/achievements/ismayeelkhan411/hawkeye/ 
