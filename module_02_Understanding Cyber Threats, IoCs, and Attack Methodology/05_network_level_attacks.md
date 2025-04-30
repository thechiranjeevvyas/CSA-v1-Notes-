# 🛠️ Network Level Attacks

## 5️⃣.1️⃣ Reconnaissance Attacks 🔍

### 📌 What is it?

Attackers gather information about a target network, including services, vulnerabilities, and system details.

### 🎯 Objectives:

- Collect network, system, and organizational information.
- Identify network blocks, intrusion detection systems, and access control mechanisms.
- Gather personal details (names, emails, job roles) for social engineering.

### 🛠️ Attack Techniques:

- **Collecting Network Information**: WHOIS lookups, traceroute.
- **Collecting System Information**: Finding vulnerabilities before launching an attack.
- **Collecting Organization’s Information**: Extracting details from websites and public records.

### 🛑 Types of Reconnaissance Attacks:

- **Active Reconnaissance** 🔴: Port scanning, OS scanning.
- **Passive Reconnaissance** 🟢: Sniffing, monitoring network traffic without detection.

### ⚠️ Examples:

- **Packet Sniffing** 📡: Capturing data packets to extract sensitive info.
- **Port Scanning** 🛑: Identifying open ports for exploitation.
- **Ping Sweeping** 📶: Finding live hosts via ICMP requests.
- **DNS Footprinting** 🌐: Using DNS queries to extract domain details.
- **Social Engineering** 🎭: Manipulating people into revealing confidential info.

---

## 5️⃣.2️⃣ Network Scanning 🔦

### 📌 What is it?

Scanning a network to find live hosts, services, firewalls, and vulnerabilities.

### 🛠️ Tools Used:

- **Nmap** 🖥️
- **Nessus** 🔍
- **OpenVAS** 🛑
- **Qualys FreeScan** ⚙️

### 🔍 What Attackers Look For:

- Active hosts & open ports
- OS & firewall details
- Vulnerable applications

---

## 5️⃣.3️⃣ Port Scanning 🎯

### 📌 What is it?

Identifying open ports on a system by sending packets to target services.

### 🔍 Why is it dangerous?

- Attackers can exploit open ports to inject malware.
- Misconfigured services provide backdoor access.

### 🛠️ Tools Used:

- **Nmap** 📡
- **Netscan Tools Pro** 🔧
- **SuperScan** 🛠️
- **PRTG Network Monitor** 📊

---

## 5️⃣.4️⃣ DNS Footprinting 🌍

### 📌 What is it?

Extracting DNS records to identify key hosts and launch further attacks.

### 🔍 What Attackers Can Discover:

- Domain names
- IP addresses
- System locations

### 🔧 Common Tools:

- WHOIS queries
- DNS lookup tools

---

## 5️⃣.5️⃣ Network Sniffing 📡

### 📌 What is it?

Capturing and analyzing network packets to extract sensitive data.

### 🛠️ Attack Methods:

- **Internal Sniffing** 🏢: Attackers inside an organization capture traffic.
- **External Sniffing** 🌍: Hackers intercept packets at the firewall.
- **Wireless Sniffing** 📶: Attacks via open Wi-Fi networks.

### 🔓 Data Stolen:

- Passwords (Telnet, FTP, email, etc.)
- Router & DNS configurations
- Chat & web traffic

---

## 5️⃣.6️⃣ Man-in-the-Middle Attack 🎭

### 📌 What is it?

Attackers secretly relay and possibly alter communication between two parties.

### ⚠️ Common Targets:

- Login pages 🔑
- Unencrypted websites 🌐
- Financial transactions 💳

### 🔧 How Attackers Perform MiTM:

- **Snooping** 👀: Listening to data traffic.
- **Intruding** 🔗: Modifying transmitted information.

---

## 5️⃣.7️⃣ Password Attacks 🔓

### 📌 What is it?

Cracking or stealing passwords to gain unauthorized access.

### 🎯 Attack Objectives:

- Steal sensitive data 💳
- Modify or deface websites 🖥️
- Gain system privileges 🔑

### 🔍 Common Techniques:

- **Dictionary Attack** 📖: Uses a list of common passwords to guess the correct one.
- **Brute Force Attack** 🔨: Tries all possible combinations of characters until the password is cracked.
- **Hybrid Attack** 🔄: Combines dictionary attacks with number and symbol variations.
- **Birthday Attack** 🎂: Exploits hash function collisions to find passwords faster.
- **Rainbow Table Attack** 🌈: Uses precomputed hash tables to quickly crack passwords.
- **Phishing** 🎣: Tricking users into revealing their passwords.
- **Credential Stuffing** 🔐: Using stolen credentials from one site to access another.
