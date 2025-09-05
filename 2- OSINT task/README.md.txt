

# 🕵️ OSINT Investigation Report – **DarkWebX**

## 🔹 Introduction

As part of the **Sprints x Microsoft Summer Cybersecurity Bootcamp**, an OSINT investigation was conducted on the cybercriminal alias **DarkWebX**. The goal was to map their digital footprint, uncover social media activity, emails, breached credentials, and IP traces — all using ethical and legal OSINT techniques.

---

## 🔹 Methodology

Tools used:
🔎 **Sherlock** · **theHarvester** · **HaveIBeenPwned** · **Hudson Rock** · **IntelligenceX** · **Google Dorking**

---

## 🔹 Key Findings

### 👤 Social Media (SOCMINT)

* Alias `DarkWebX` flagged on **29 platforms**.
* ✅ Verified: [Reddit](https://www.reddit.com/user/DarkWebX) (active).
* 🔗 Hudson Rock confirmed leaked credentials linked to this username.
* The rest: inactive/dormant.

---

### 📧 Email Addresses

* Found: `yourusername@protonmail.com`.
* Checked via **HaveIBeenPwned** → **No confirmed breaches**.

---

### 💀 Breached Credentials

Hudson Rock linked **DarkWebX** to 2 stealer-infected systems:

| 📅 Date  | 🦠 Stealer | 💻 OS / Device  | 🌍 IP (partial) |
| -------- | ---------- | --------------- | --------------- |
| Feb 2024 | Lumma      | Windows 10 x64  | `138.94.*.*`    |
| Jan 2024 | RedLine    | Windows 10 Home | `201.218.*.*`   |

🔐 Exposed obfuscated credentials (emails + passwords).

---

### 🌍 IP Addresses

Extracted from leaked dumps & OSINT tools:

* `74.50.94.211` 🇺🇸 US
* `129.205.113.199` 🇳🇬 Nigeria
* `152.110.151.79` 🇿🇦 South Africa
* `111.95.44.115` 🇮🇩 Indonesia
* `146.70.104.254` 🇬🇧 UK
* More in `screenshots/`

---

## 🔹 Conclusion

The alias **DarkWebX** shows:
✔️ Active Reddit presence.
✔️ Linked to **info-stealer malware infections**.
✔️ Multiple IPs tied to leaked data & malware dumps.

This highlights the risks of compromised credentials and provides a profile of the actor’s exposed footprint.

---

## 🧩 Attribution

Report prepared during the **OSINT phase** of the **Sprints x Microsoft Summer Cybersecurity Bootcamp** using **publicly available intelligence sources only**.
