# 📌 Indicators of Compromise (IoCs)

## 🧠 Why IoCs are Important?

Indicators of Compromise (IoCs) are forensic evidence that organizations can use to detect malicious activities at an early stage. These red flags can help in identifying potential breaches or attacks before they cause significant harm.

🔍 **Key Reasons to Analyze IoCs:**

- 🛡️ Detect data breaches, malware intrusions, and suspicious activity.
- 🧬 Understand the behavior and characteristics of malware.
- ⚡ Enhance threat response time and detection rates.
- ⚙️ Feed automated tools with data for proactive scanning and protection.
- ❓ Answer crucial questions like:
  - Does the file contain malicious content?
  - Is the organization compromised?
  - How did the infection occur?

🔔 **Suspicious Indicators:**

- Application delays in rendering database/web server pages.
- FTP/HTTP logs showing unusual outbound connections.

---

## 🔎 8.2. IoC Detection Techniques

### 🛠️ 8.2.1. SQL Injection Attempts

**How to Detect:**

- Examine log files of IDS, web servers, and databases.
- Check for suspicious SQL queries, such as:
  - `GET /login.asp?username=blah' or 1=1 --`
  - `GET /login.asp?username=blah' or exec master.xp_cmdshell 'net user ...'`

---

## 🚨 8.4. IoC Detection Techniques (Expanded)

### 🌐 Monitoring Network Traffic

**Why:**
Every activity over the network creates traffic. Monitoring helps detect irregular patterns.

**What to Monitor:**

- IP/MAC addresses, protocols, ports, URLs, file sizes.
- Spikes/drops in bandwidth, QoS, and network speeds.
- Use tools like **Wireshark**, **Colasoft Network Analyzer**, **Observer Analyzer**.

### 🧪 Sniffing Network Traffic

**Purpose:**
Identify victim/source devices and propagation methods.

**Tools:**

- **Wireshark**, **Tcpdump**, **Cain & Abel**, **Kismet**
- Set baseline for normal traffic before sniffing.

### 📦 Performing Packet Analysis

**What to Analyze:**

- IP addresses, ports, DNS, TTL, SSL certificates
- TCP anomalies, IRC traffic, time-based connections

**Tools:**

- **NetworkMiner**, **ngrep**, **hex editors**, **Sniff**, **Ettercap**, **OmniPeek**, **Tepdump**

### 📋 Performing Log Analysis

**Why:**
Logs provide timeline-based evidence of system actions.

**Tips:**

- Use filters and tools to analyze large volumes.
- Preserve original logs to maintain integrity.

### 🖥️ Performing Host Analysis

**Goal:**
Detect malicious processes, services, and binaries on host machines.

**How:**

- Look for unusual processes or suspicious binaries.
- Perform static/dynamic analysis to understand behavior.

---

## ✅ Detection Outcomes

- 🔍 Detection of malicious sniffers
- ⚠️ Misconfigurations like routing/DNS leaks
- 🚨 Suspicious protocol behavior (invalid bits, fragments)
- 🧬 Malicious fingerprinting or firewall/proxy bypass attempts

---

> "A network without proper IoC monitoring is like a fortress with its gates open."

---

✅ **Stay vigilant, monitor constantly, and respond swiftly to protect your organization's network.**
