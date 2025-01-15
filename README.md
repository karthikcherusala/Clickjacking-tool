<h1 align="center">Clickjacking Tester Tool</h1>

<p align="center">
  A Bash script to test websites for clickjacking vulnerabilities by embedding them in an iframe. 
</p>

---

## 🔍 About
This tool helps to check if a website is vulnerable to **clickjacking attacks**. It generates an HTML page embedding the target URL in an iframe. If the website loads successfully, it may be vulnerable.

---

## 🚀 Features
- Easy-to-use Bash script for Linux systems.
- Checks for clickjacking vulnerabilities by rendering target sites in an iframe.
- Supports popular browsers:
  - Google Chrome
  - Firefox
  - Brave

---

## ⚙️ Prerequisites
Ensure the following browsers are installed:
- **Google Chrome**: `sudo apt install google-chrome-stable`
- **Firefox**: `sudo apt install firefox`
- **Brave Browser**: [Install Brave](https://brave.com/linux/)

---

## 📦 Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/clickjacking-tool.git
   cd clickjacking-tool
