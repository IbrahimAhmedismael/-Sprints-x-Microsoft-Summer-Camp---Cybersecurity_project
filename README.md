

# 🚀 Sprints x Microsoft – Summer Cybersecurity Bootcamp

This repo contains my practical solutions to the **SOC** 🛡️ and **OSINT** 🔎 cybersecurity challenges from the Sprints x Microsoft Summer Bootcamp.

---

## 🛡️ 1. SOC Task – Malware Forensics

### 🖥️ Setup

* Isolated **Windows 10 VM** (Defender & updates disabled)
* Malware executed for **60s**
* **Memory + Network** captured with FTK Imager & Wireshark

### 🛠️ Tools

Wireshark · Volatility 3 · FTK Imager · YARA · VMware

### 🔍 Key Findings

* **🌐 Network:**

  * Malformed DNS → `85.114.128.127`
  * HTTP GET to `23.12.131.222` (fake Flash Player update)

* **💾 Memory:**

  * Hidden `cmd.exe` (PID 6296)
  * Code injection in `SearchApp.exe` & `MsMpEng.exe`
  * Fake `msedgewebview2.exe` spawning `SearchApp.exe`

* **⚠️ IOCs:**

  * RWX memory injections
  * Hidden process activity
  * Suspicious WebView-based browser process

---

## 🔎 2. OSINT Task – Tracking **DarkWebX**

### 🎯 Objectives

* Identify accounts, emails, breached data & IPs using OSINT

### 🛠️ Tools

Sherlock · theHarvester · HaveIBeenPwned · Hudson Rock · Google Dorks · WHOIS

### 🔍 Key Findings

* **👤 Social Media:** 29 accounts flagged → only **Reddit** active
* **📧 Email:** One ProtonMail found (no confirmed breaches)
* **💀 Breached Data:** Linked to **Lumma (Feb 2024)** & **RedLine (Jan 2024)** stealers
* **🌍 IPs:** Multiple traced (US, NG, ZA) from leaked logs & infostealer dumps

---

## 📂 Repo Structure

```
Sprints-x-Microsoft-Summer-Cybersecurity-Bootcamp/
│
├── 1- SOC task/
│   ├── reports/ 
│   ├── screenshots/
│   └── volatility outputs/
│
└── 2- OSINT task/
    ├── osint_report
    └── screenshots/

