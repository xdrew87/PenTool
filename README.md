

# 🛡️ PenTest CLI Tool

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<p align="center">
  <img src="https://raw.githubusercontent.com/yourusername/yourrepo/main/banner.png" alt="PenTest CLI Tool Banner" width="600">
</p>

---

## 🚀 Overview

**PenTest CLI Tool** is a powerful, modular, and visually appealing command-line toolkit for professional penetration testers and cybersecurity enthusiasts. It automates a wide range of recon and assessment tasks, making it ideal for both quick scans and deep analysis.

---

## ✨ Features

<details>
<summary>Click to expand</summary>

- 🔍 **TCP & UDP Port Scanning** — Customizable, fast, and reliable
- 🕵️ **Service Detection** — Banner grabbing, protocol checks
- 🛡️ **Vulnerability Checks** — CVE lookup for detected services
- 🌐 **Subdomain Enumeration** — Finds common subdomains
- 🧩 **Web Directory/File Brute-Forcing** — Discovers hidden endpoints
- 📄 **HTTP(s) Info** — Headers, SSL certificate, supported methods
- 🗂️ **DNS Enumeration** — A, MX, TXT, NS records
- 🖥️ **OS Detection** — TCP/IP fingerprinting
- 📝 **Logging** — Save results to file
- 🎨 **Colorized Output** — Easy to read, visually appealing
- ⚡ **Scan Speed Control** — Tweak for stealth or speed

</details>

---

## ⚡ Quickstart

### 1. Install Requirements

```bash
pip install requests colorama dnspython
```

### 2. Run a Scan

```bash
python pentest_cli.py <target> [--ports 80,443,8080] [--udp-ports 53,123] [--scan-speed 0.5] [--log results.txt]
```

#### Example

```bash
python pentest_cli.py example.com --ports 80,443,8080 --udp-ports 53,123 --scan-speed 0.2 --log pentest_results.txt
```

---

## 🛠️ Arguments

| Argument      | Description                                      |
|-------------- |--------------------------------------------------|
| `target`      | Target IP or domain to scan                      |
| `--ports`     | Comma-separated TCP ports to scan (default: common ports) |
| `--udp-ports` | Comma-separated UDP ports to scan (default: common UDP ports) |
| `--scan-speed`| Scan speed in seconds (default: 0.5)             |
| `--log`       | Log output to file                               |

---

## 📋 What It Does

- Scans TCP and UDP ports
- Detects services and grabs banners
- Checks for known vulnerabilities (CVE links)
- Enumerates common subdomains
- Brute-forces common web directories/files
- Fetches HTTP info and SSL certificate details
- Enumerates DNS records (A, MX, TXT, NS)
- Attempts OS detection via TCP/IP fingerprinting
- Logs all results to file if specified

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## 📄 License

MIT

---

> **Disclaimer:** This tool is for educational and authorized security testing purposes only. Use responsibly and always obtain proper permission before scanning any system.
