# 🔐 Network Scanning & Vulnerability Assessment using Kali Linux (VirtualBox)

This project demonstrates the **network scanning**, **device enumeration**, and **basic vulnerability assessment** process using **Kali Linux** on **VirtualBox**, designed for **students and entry-level cybersecurity practitioners**. All scans were performed in a **controlled environment** using only a laptop and mobile hotspot — perfect for beginners and internship-level proof-of-concept.

---

## 🚀 Project Overview

- 🔍 **Discover devices** in the network using `Netdiscover`  
- 🌐 **Scan for open ports** and running services using `Nmap`  
- 🛡️ **Perform vulnerability scan** on a test web server using `Nikto`  
- 📸 Includes screenshots of command outputs for easy understanding  
- 📝 Generates a professional report (`.txt`) for documentation or portfolio

---

## 🧰 Tools Used

| Tool        | Purpose                              |
|-------------|------------------------------------|
| Netdiscover | Network discovery                   |
| Nmap        | Port and service enumeration        |
| Nikto       | Web server vulnerability scanning   |

---

## 🖥️ Environment Setup

- ✅ **Kali Linux** (running in VirtualBox)  
- ✅ Internet connection via **Mobile Hotspot**  
- ✅ **No extra devices** required — scanning performed on local and test targets  
- ✅ Host system: **Windows 10/11**

---

## 📂 Project Structure

```bash
network-scanning-kali/
│
├── nmap_scan.txt
├── nikto_report.txt
├── README.md
└── screenshots/
    ├── nmap_screenshot.JPG
    ├── nikto_screenshot.JPG
    └── netdiscover_screenshot.JPG
````

---

## 📸 Screenshots

Include the following screenshots for better visual understanding:

* ![Nmap Screenshot](screenshots/nmap_screenshot.JPG) – result showing detected ports and services
* ![Nikto Screenshot](screenshots/nikto_screenshot.JPG) – Nikto vulnerability scan output
* ![Netdiscover Screenshot](screenshots/netdiscover_screenshot.JPG) – devices found on the network by Netdiscover

---

## 🔍 Step-by-Step Scanning Process

### 1️⃣ Discover Devices with Netdiscover

```bash
sudo netdiscover
```

> Used to identify IP addresses, MAC addresses, and vendors on the local network.

📁 Output: ![Netdiscover Screenshot](screenshots/netdiscover_screenshot.JPG)

---

### 2️⃣ Scan for Open Ports using Nmap

```bash
sudo nmap -A <target-ip>
```

* `-A` enables OS detection, version detection, script scanning, and traceroute.
* Look for open ports and services (e.g., 80/tcp, 22/tcp).

📁 Output: [nmap\_scan.txt](nmap_scan.txt), ![Nmap Screenshot](screenshots/nmap_screenshot.JPG)

---

### 3️⃣ Scan Web Server Vulnerabilities using Nikto

```bash
nikto -h http://testphp.vulnweb.com
```

* A public vulnerable test server (no legal issues)
* Checks for common web server misconfigurations, open directories, outdated software

📁 Output: [nikto\_report.txt](nikto_report.txt), ![Nikto Screenshot](screenshots/nikto_screenshot.JPG)

---

## 🧾 Final Outputs (Reports)

* [nmap\_scan.txt](nmap_scan.txt) – Details of open ports, services, and possible OS
* [nikto\_report.txt](nikto_report.txt) – Report of web vulnerabilities found on test server

📎 *These are helpful for attaching in internship reports, assignments, or resumes.*

---

## 💡 Learning Outcomes

✅ Hands-on experience with real cybersecurity tools
✅ Understand basic network enumeration and scanning logic
✅ Build a small portfolio project without needing enterprise hardware
✅ Learn documentation and project structuring for GitHub/LinkedIn

---

## 📌 Note

* All scans were conducted in a **safe, legal, and isolated test environment**
* Screenshots and reports are for **educational and demonstration** purposes only

---

## 🧠 Author

**Inishi Dinethma**
BSc (Hons) in Computer Networks – NSBM Green University
🔗 [LinkedIn Profile](http://linkedin.com/in/inishi-dinethma-852376264)

---

## 🏷️ Tags

`#KaliLinux` `#Cybersecurity` `#NetworkScanning` `#Nmap` `#Nikto` `#Netdiscover` `#BeginnerProject` `#InternshipPortfolio`
