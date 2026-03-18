# Project 2: SIEM Correlation Rules

## 📌 Objective
Develop and test custom correlation rules in a SIEM (Splunk) to detect:
- Credential Stuffing  
- DNS Tunneling  
- PowerShell Exploitation  

Thiss project was part of my internship where the goal was to simulate common attack techniques and build detection mechanisms using SIEM tools.

---

## 🛠️ Tools Used
- **Splunk Cloud** (SIEM platform)
- Simulated log files (for Credential Stuffing, DNS Tunneling, PowerShell Exploitation)

---

## 📊 Methodology
1. Created and ingested simulated log files for each attack technique.
2. Built correlation search queries in Splunk.
3. Configured alerts to trigger when suspicious activity was detected.

---

## 🔍 Detection Rules

### 1️⃣ Credential Stuffing
**Logic:** Detect multiple failed login attempts from the same IP within a short time window.  
**Query Screenshot:**  
![Credential Stuffing Query](https://github.com/IsmayeelKhan77/Internship-Project-2-SIEM-Correlation-Rules/blob/main/screenshots/Credential_stuffing%20ss1.png?raw=true)  
**Alert Configuration Screenshot:**  
![Credential Stuffing Alert]( https://github.com/IsmayeelKhan77/Internship-Project-2-SIEM-Correlation-Rules/blob/main/screenshots/credential_stuffing%20ss2.png?raw=true)  

---

### 2️⃣ DNS Tunneling
**Logic:** Detect abnormal frequency of DNS queries to the same suspicious domain within a small timeframe.  
**Query Screenshot:**  
![DNS Tunneling Query](https://github.com/IsmayeelKhan77/Internship-Project-2-SIEM-Correlation-Rules/blob/main/screenshots/dns_tunneling%20ss1.png?raw=true)  
**Alert Configuration Screenshot:**  
![DNS Tunneling Alert](https://github.com/IsmayeelKhan77/Internship-Project-2-SIEM-Correlation-Rules/blob/main/screenshots/dns_tunneling%20ss2.png?raw=true
)  

---

### 3️⃣ PowerShell Exploitation
**Logic:** Detect suspicious PowerShell commands (e.g., encoded commands, remote execution attempts).  
**Query Screenshot:**  
![PowerShell Query](https://github.com/IsmayeelKhan77/Internship-Project-2-SIEM-Correlation-Rules/blob/main/screenshots/PowerShell%20Exploitation%20ss1.png?raw=true)  
**Alert Configuration Screenshot:**  
![PowerShell Alert](https://github.com/IsmayeelKhan77/Internship-Project-2-SIEM-Correlation-Rules/blob/main/screenshots/PowerShell%20Exploitation%20ss2.png?raw=true)  

---

## ✅ Outcome
- Successfully simulated attack techniques.  
- Built correlation rules and alerts in Splunk.  
- Screenshots provide evidence of detection rules and alert creation.  

---

## 🚀 Next Steps 
- Explore more advanced attack detection (e.g., lateral movement, privilege escalation).

