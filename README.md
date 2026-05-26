# NetGuard – Threat Detection Bot

## Project Overview

NetGuard is a Python-based real-time network monitoring and threat detection system.
The project captures live network packets, analyzes traffic behavior, detects suspicious activities, generates alerts, and stores threat logs for security monitoring.

Used Library:
- Scapy

---

# Features

- Live packet sniffing
- Source and destination IP extraction
- Protocol identification
- Packet size monitoring
- Suspicious activity detection
- High bandwidth detection
- Unauthorized IP detection
- Alert generation
- Threat logging
- Unit test case implementation
- Exception logging

---

# Technologies Used

- Python
- Scapy
- VS Code
- GitHub

---

# Project Structure

NetGuard/

│

├── main.py

├── requirements.txt

├── README.md

│

├── services/

│   ├── __init__.py

│   ├── packet_sniffer.py

│   └── detector.py

│

├── utils/

│   ├── __init__.py

│   ├── alerts.py

│   └── logger.py

│

├── config/

│   ├── __init__.py

│   └── config.py

│

├── tests/

│   └── test_detector.py

│

├── logs/

│   └── threat_logs.txt

---

# Module Description

## main.py
Entry point of the application.

## packet_sniffer.py
Captures live network packets and extracts packet details.

## detector.py
Detects suspicious activities, unauthorized access, and high bandwidth usage.

## alerts.py
Generates alert messages.

## logger.py
Stores threat details into log files.

## config.py
Stores threshold values and trusted IP addresses.

## test_detector.py
Validates threat detection scenarios using unit test cases.

---

# Threats Detected

## 1. Unauthorized Access
Detects unknown IP addresses.

## 2. Suspicious Activity
Detects repeated requests from the same IP.

## 3. High Bandwidth Usage
Detects abnormal packet size and traffic usage.

---

# Run The Project

```bash
python main.py
```

---

# Run Unit Test Cases

```bash
python tests/test_detector.py
```

---

# Sample Output

```plaintext
[ALERT] Unauthorized Access detected from IP: 192.168.55.1

[ALERT] High Bandwidth Usage detected from IP: 192.168.1.101
```

---

# Logging

Threat details are stored in:

```plaintext
logs/threat_logs.txt
```

Logged Details:
- Timestamp
- Threat Type
- IP Address
- Packet Size
- Protocol

---

# Future Enhancements

- Email alert system
- Dashboard visualization
- Machine learning-based threat detection
- Database integration
- Real-time monitoring dashboard

---

# Conclusion

NetGuard is a modular real-time network threat detection system that improves network monitoring by identifying suspicious traffic behavior and generating security alerts