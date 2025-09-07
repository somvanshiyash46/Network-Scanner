🌐 Network Scanner 🔍

A Python-based Network Scanner ⚡ that helps network administrators 👨‍💻, ethical hackers 🕵️‍♂️, and security professionals 🛡️ discover hosts, analyze network configurations, and detect potential vulnerabilities.

This tool leverages Scapy 🐍 for packet crafting and supports multiple scanning techniques including ICMP, TCP, and ARP. Whether you’re checking availability, finding open ports, or mapping devices on a subnet, this scanner is built to deliver fast ⚡ and reliable results.

✨ Features

✅ ICMP Echo Request (Ping) Scanning 📡 – Quickly check if hosts are alive
✅ TCP Port Scanning 🔌 – Identify open ports and running services
✅ ARP Network Scanning 🖧 – Discover devices on local networks
✅ Configurable Scan Types & Timeouts 🎛️ – Full flexibility for precise scans
✅ Port Range Support 🎯 – Scan single ports, lists, or ranges (1–65535)
✅ Detailed Scan Results 📑 – Clear IP + MAC mapping for each device

📦 Requirements

🐍 Python 3.6+

📡 Scapy 2.5.0+ (for packet manipulation)

🔑 Root/Admin Privileges (required for raw socket operations)

⚙️ Installation

Clone the repo and install dependencies:

git clone https://github.com/yourusername/network-scanner.git
cd network-scanner
pip install -r requirements.txt

🚀 Usage

Run the scanner from the command line:

python main.py -ip <target>

🔍 Examples

1️⃣ Scan a single host

python main.py -ip 192.168.1.1


2️⃣ Scan a subnet using ARP

python main.py -ip 192.168.1.0/24


3️⃣ Check only with ICMP

python src/main.py 192.168.1.1 -t icmp


4️⃣ Port scanning specific services

python src/main.py 192.168.1.1 -p 80,443,8080


5️⃣ Port range scanning

python src/main.py 192.168.1.1 -p 1-1000

📂 Project Structure
network-scanner/
├── src/
│   ├── main.py         # Command-line interface
│   └── scanner.py      # Core scanning functionality
├── tests/              # Unit tests
├── docs/               # Documentation
├── requirements.txt    # Project dependencies
├── requirements-dev.txt# Dev/test dependencies
├── setup.py            # Package setup
└── README.md           # Documentation

⚠️ Security Considerations

⚡ Intrusive Nature – Network scanning may be flagged as suspicious or intrusive.
🔒 Permissions – Use ONLY on networks you own or have explicit authorization to scan.
🚫 Restrictions – Some firewalls and routers may block ICMP, TCP, or ARP traffic.
🔑 Privileges Required – Running requires root/administrator rights.

🛡️ License

📜 This project is licensed under the MIT License – feel free to use, modify, and share with proper credit.

🔥 With this scanner, you get a lightweight yet powerful tool to quickly map out your network and strengthen your security posture.
