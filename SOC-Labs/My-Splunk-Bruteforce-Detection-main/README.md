# Brute Force Login Detection 

**Goal:** Detect repeated failed login attempts (possible brute force) using Splunk Cloud and a public dataset, and prove it with a working alert.

---

## What this project shows
- I ingested a public dataset into Splunk Cloud.
- I wrote an SPL detection for brute force attempts.
- I converted the search into a scheduled alert (cron).
- The alert triggers and can be triaged (screenshots below).

---

## Dataset (source & context)
- Source: Splunk Attack Data (O365 sign-in style logs, JSON format).
- I uploaded the JSON file via **Search & Reporting → Add Data → Upload file**.
- Index used: `main` (cloud trials sometimes restrict custom indexes).

> Why O365 brute force? It’s one of the most common real-world attacks against user accounts. Repeated failed logins from the same IP against the same user is a strong early signal.

---

## SPL detection query

> Set time range to **Last 5 minutes** before saving as an alert.

```spl
index=main ResultStatus="Failed"
| stats count as failed_attempts values(ActorIpAddress) as IPs by "Actor{}.ID"
| where failed_attempts > 5
