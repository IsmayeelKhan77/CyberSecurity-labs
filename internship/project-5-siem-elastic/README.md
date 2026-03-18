# Project 5 — Custom SIEM Dashboard (Elastic)

**Author:** Ismayeel  
**Project:** Build a simple SIEM dashboard (Elastic) that shows brute-force, privilege escalation and possible exfiltration.

---

## Short summary
I built a small SIEM dashboard in Elastic (Kibana) that shows:
- Brute-force attempts (failed logins)
- Privilege escalation events (sudo, commands)
- Potential data exfiltration (curl/wget/scp)
- Login success vs failure

This was made as part of my internship project.

---

## Index / Data
- **Index / Data view used:** `siem_index`  
  (When creating visualizations in Lens, pick this data view.)

---

## KQL / Filters I used (copy-paste into Kibana Discover or Lens filter bar)

**Brute-force (failed logins)** 
message:("Failed password" OR "Failed login")

**Privilege escalation (sudo / elevated commands)**  
message:(sudo OR "COMMAND=" OR "root")

**Possible exfiltration (download/transfer commands)**  
message:(curl OR wget OR scp OR rsync OR ftp)

**Successful logins**  
message:("Accepted password" OR "Accepted publickey" OR "session opened")


---


## How to use / reproduce quickly
1. Open Kibana → Visualize (Lens) and choose the data view.  
2. Paste the KQL filters above in the query bar to test.  
3. Create visualizations per the titles above and then add them to a dashboard.  
4. Save the dashboard as: **SIEM Dashboard – Security Events Overview**

---

## Notes / Evidence
- This is a basic detection/dashboard setup made with internship data. It shows good coverage for common stuff like brute-force, sudo, and command-based exfiltration.
- Screenshots are in the Screenshot folder.
