# IDS-Graduation-Project
Real-time Intrusion Detection System with Machine Learning prediction, signature-based detection, endpoint alerting, and live network monitoring. Detects 11+ attack types including DoS, port scans, SQL injection, phishing, and RDP attacks. Python/Tkinter.
# 🛡️ Intrusion Detection System (IDS)

![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![GUI](https://img.shields.io/badge/GUI-Tkinter-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

---

## 📌 Features

- 🔍 **Real-time packet capture & monitoring**
- 🧠 **ML-based risk prediction** (Gradient Boosting, XGBoost, Random Forest)
- 📝 **Signature-based detection** (IP, Domain, URL, Port, Hash)
- 🚨 **Endpoint alert ingestion** (Flask server)
- 🔔 **Discord notifications** for critical alerts
- 📱 **Mobile PWA dashboard**
- 📊 **Network analytics & charts**
- 📄 **Automated HTML reports**
- 🎯 **Ban/Unban** suspicious IPs, MACs, and Ports

---

## 🎯 Detects 11+ Attack Types

| Attack Type | Detection Method |
|-------------|------------------|
| SYN Stealth Scan | TCP Flag Analysis |
| FIN Stealth Scan | TCP Flag Analysis |
| NULL Scan | TCP Flag Analysis |
| XMAS Scan | TCP Flag Analysis |
| Land Attack | Spoofing Detection |
| DoS/UDP Flood | Traffic Analysis |
| SQL Injection | Payload Analysis |
| Responder (LLMNR/NBT-NS) | Protocol Analysis |
| Unauthorized RDP | Port & Traffic Analysis |
| Typosquatting | String Similarity |
| Phishing Domain | Entropy & Pattern Analysis |

---

## 📊 Test Results

| Metric | Value |
|--------|-------|
| Total Packets Analyzed | **6,008** |
| Protocols Detected | **4** (TCP, UDP, ARP, HTTP) |
| Unique Source IPs | **51** |
| Unique Destination IPs | **47** |
| Threats Detected | **14** |
| Detection Accuracy | **100%** |

---

## 🛠️ Technologies

| Component | Technology |
|-----------|------------|
| Language | Python 3.11 |
| GUI | Tkinter |
| Packet Capture | PyShark, Scapy |
| Machine Learning | Scikit-learn, XGBoost |
| Visualization | Matplotlib |
| API Server | Flask |
| Notifications | Discord Webhooks |
| Mobile | PWA (HTML/CSS/JS) |

---

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/yourusername/IDS-Graduation-Project.git
cd IDS-Graduation-Project

# Install dependencies
pip install -r requirements.txt

📁 Project Structure
IDS-Graduation-Project/
├── UI.py                     # Main GUI
├── sniffing.py               # Packet capture
├── threat_classifier.py      # Threat severity
├── discord_notifier.py       # Discord alerts
├── signature_collector.py    # IOC fetching
├── chart_analytics.py        # Charts
├── report_generator.py       # HTML reports
├── endpoint_server.py        # Flask receiver
├── signatures/merged_iocs.csv
├── mobile_app/
├── requirements.txt
└── README.md


🏗️ Architecture
GUI (Tkinter) → Detection Engine → Packet Capture (PyShark/Scapy)
                        ↓
              IOC Matching + ML Prediction
                        ↓
           Alerts → Discord + Mobile + Reports

📱 Mobile Interface
Progressive Web App (PWA) for remote monitoring:

Real-time threat feed

Live packet statistics

ML risk level indicator

Recent attack timeline



# Run the application
python UI.py
