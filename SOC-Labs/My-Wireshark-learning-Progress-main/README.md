# Wireshark Basics 🚀

## 📖 Objective
As a 17-year-old beginner in cybersecurity, I wanted to explore how network traffic works using **Wireshark**.  
The goal of this project is **not advanced packet analysis**, but simply to learn the basics, capture some packets, and document the process as a proof of skill.

This repository contains my first hands-on practice with:
- DNS (Domain Name System)
- ICMP (Internet Control Message Protocol)
- TLS (Transport Layer Security)

---

## 🛠️ Tools Used
- **Wireshark** (for packet capturing and analysis)
- **My own WiFi network** (to generate real traffic)
- **Basic networking commands** like ping

---

## 🌐 What I Did

### 1. DNS (Domain Name System)
- **What it is:** DNS is like the phonebook of the internet. It translates domain names (like `google.com`) into IP addresses.  
- **What I did:** I applied the filter `dns` in Wireshark and visited some websites.  
- **What I saw:** Queries being sent to resolve domain names.
- 

---

### 2. ICMP (Ping Protocol)
- **What it is:** ICMP is used to check connectivity between devices (example: the `ping` command).  
- **What I did:** I pinged `8.8.8.8` (Google DNS) and captured the traffic in Wireshark with filter `icmp`.  
- **What I saw:** ICMP Echo Request and Echo Reply packets going back and forth.  

---

### 3. TLS (Transport Layer Security)
- **What it is:** TLS encrypts communication between client and server (like HTTPS).  
- **What I did:** I opened some HTTPS websites and used the filter `tls` in Wireshark.  
- **What I saw:** TLS handshake (Client Hello, Server Hello) and encrypted data.  

---

## Proof of skill:
- I'm putting every screenshot in separate files, you can check it out if you want.
---

## 📌 Key Learnings
- Every website visit creates **DNS queries**.  
- **Ping** uses ICMP packets, which are very easy to spot in Wireshark.  
- Secure websites use **TLS**, so the content is encrypted (cannot be read in plain text).  

---

## 🧑‍💻 Why This Repo?
This is my **first networking project**. I kept it simple to show that:
- I can set up Wireshark
- I understand the basics of packet analysis
- I can document and share my learning process

---

## 🚀 Future Plans
- Explore **ARP traffic** (Address Resolution Protocol)  
- Perform a safe **Nmap scan** in a controlled environment  
- Learn about **HTTP vs HTTPS differences**

---


