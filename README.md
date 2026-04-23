🔥 GitHub Repo (README.md)

You can name your repo something like:
👉 tryhackme-fakebank-splunk-botsv3-lab

📄 README.md
# 🛡️ TryHackMe FakeBank + Splunk BOTS v3 SOC Analysis

This project documents my hands-on experience combining **Offensive Security (TryHackMe FakeBank lab)** with **Defensive Security using Splunk BOTS v3 dataset**.

---

## 🚀 Objective

- Perform web enumeration using Gobuster
- Discover hidden directories on a target machine
- Simulate attacker behavior
- Analyze real-world logs using Splunk (BOTS v3 dataset)
- Understand SOC investigation workflow

---

## 🧰 Tools & Technologies

- Kali Linux
- Gobuster
- TryHackMe (FakeBank Lab)
- Splunk Enterprise
- BOTS v3 Dataset
- Linux CLI

---

## ⚔️ Part 1: Offensive Security (FakeBank Lab)

### 🔍 Command Used

```bash
gobuster dir -u http://fakebank.thm -w wordlist.txt
📌 Findings
/images → Redirect (301)
/bank-transfer → Accessible (200)
💡 Key Learning
Directory brute-forcing helps uncover hidden endpoints
Status codes help identify valid paths
Real-world attackers use similar techniques
🛡️ Part 2: Defensive Security (Splunk BOTS v3)

Dataset: Splunk Boss of the SOC (BOTS) v3

🔍 Search Query
index=botsv3 earliest=0
📊 Data Sources Explored
AWS CloudTrail Logs
Windows Event Logs (Sysmon)
DNS / HTTP Traffic
Linux Logs
Network Traffic (PCAP-based logs)
🧠 SOC Investigation Skills Practiced
Log analysis & correlation
Identifying suspicious behavior
Threat hunting basics
Understanding attacker patterns
Working with multiple log sources
⚡ Key Takeaways
Offensive skills help understand attacker mindset
Defensive tools like Splunk help detect attacks
Real SOC work = connecting logs + context
Visibility across systems is critical
📂 Project Structure
/screenshots
    gobuster-output.png
    splunk-search.png

/notes
    findings.md
📸 Screenshots

(Add your screenshots here)

🔗 References
TryHackMe Offensive Security Intro
Splunk BOTS v3 Dataset
🧑‍💻 Author

Your Name
Aspiring SOC Analyst | Cybersecurity Enthusiast