<h1 align="center">Clickjacking Tester Tool</h1>

<p align="center">
  A Bash script to test websites for clickjacking vulnerabilities by embedding them in an iframe. 
</p>

---

## 🔍 About
This tool helps to check if a website is vulnerable to **clickjacking attacks**. It generates an HTML page embedding the target URL in an iframe. If the website loads successfully, it may be vulnerable.

---
# 🛡️ What is Clickjacking?

**Clickjacking** is a type of web attack where an attacker tricks users into clicking something different from what they perceive, potentially leading to unwanted actions. A vulnerable website can be framed (embedded in an invisible iframe) on a malicious site, causing the user to unknowingly interact with the embedded site. This can lead to unintended actions, like changing settings or sharing sensitive information without their knowledge.

Clickjacking often takes advantage of websites that don’t have proper protections like **X-Frame-Options** headers, which prevent embedding in iframes.

### Example:
When a website is vulnerable, it can be loaded into an invisible frame on another website, allowing an attacker to perform actions on behalf of the victim.

---

### How to Protect Against Clickjacking:
- Use **X-Frame-Options** HTTP headers with values like `DENY` or `SAMEORIGIN` to prevent iframe embedding.
- Implement a **Content Security Policy (CSP)** with the `frame-ancestors` directive to control which domains can embed your website.

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
To install and run the tool, follow the steps below:

# Clone the repository
git clone https://github.com/karthikcherusala/clickjacking-tool.git

# Navigate to the directory
cd clickjacking-tester

# Set executable permissions for the script
chmod 755 clickjacking-tester.sh

# Copy the script to your desired directory
cp ./clickjacking-tester.sh /home/user/Downloads/

# Exit from the current directory
exit

# Navigate to the Downloads directory
cd Downloads

# Run the script
./clickjacking-tester.sh


## ⚠️ Warning
This tool only works without root privileges. Running it with root may cause issues with browser execution.

🛠️ Usage
1.Run the script:
./clickjacking_tool.sh

2.Enter the target URL when prompted.

3.Choose the browser to test the site:

1: Google Chrome
2: Firefox
3: Brave
The tool opens a test page in the selected browser to check for clickjacking.

📝 Author
Karthik

Feel free to connect with me on LinkedIn or contribute to this project!

🤝 Contributing
Contributions are welcome! Fork this repository, make your changes, and submit a pull request.

🎯 Disclaimer
This tool is for educational purposes only. Testing on websites without proper authorization is illegal and against ethical hacking practices. Always obtain permission before conducting security tests.
