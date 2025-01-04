# CodeTech-Task-2
Name : Muthumeena M 
Company : CODTECH IT SOLUTIONS 
Intern ID : CT08DIM 
Domain : Cyber Security & Ethical Hacking

**Task 2 : Vulnerability Scanning Tool**

This repository contains a simple Python-based tool for scanning network vulnerabilities. The tool includes functions for port scanning, software version checking, and misconfiguration detection (like directory listing).

**Features**

- **Port Scanning:**
  - Scans the first 1024 ports on a target IP address or domain using the `nmap` library.
  
- **Software Version Checking:**
  - Checks for outdated or vulnerable software by analyzing the banner of services running on a specific port (e.g., HTTP on port 80).
  
- **Directory Listing Check:**
  - Verifies whether directory listing is enabled on a web server, which could expose sensitive files and directories.

**Installation**

**Dependencies**
- Python 3.x
- Required libraries:
  - `nmap`: For port scanning.
  - `socket`: For establishing network connections.
  - `requests`: For HTTP requests.

Install the required libraries using pip:
bash
pip install python-nmap requests


**Clone the Repository**
bash
git clone https://github.com/Badalkathayat/vulnerability-scanning-tool.git
cd vulnerability-scanning-tool


**Usage**

Run the script using Python:

bash
python vulnerability_scanning_tool.py


You will be prompted to enter the target domain or IP address. The tool will then perform the following checks:

1. **Port Scanning:** Scans the first 1024 ports on the target.
2. **Software Version Checking:** Attempts to retrieve the banner from the web server on port 80.
3. **Directory Listing Check:** Checks if directory listing is enabled on the target web server.

**Example**

plaintext
Enter the target (domain/IP): example.com
Scanning for open ports...
Host : 192.168.1.1 (example.com)
State : up
Protocol : tcp
Port : 80   State : open

Checking for outdated software versions...
Banner: HTTP/1.1 200 OK...

Checking for misconfigurations...
Directory listing is not enabled.


**Future Enhancements**

- **Extended Port Range:** Allow scanning of additional port ranges.
- **Service Detection:** Improve software version checking by detecting more services.
- **Advanced Misconfigurations:** Add checks for other common web server misconfigurations.

**Contributing**

Contributions are welcome! Feel free to fork this repository, submit pull requests, or raise issues.

**License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
