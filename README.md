# 🛡️ RangeGuard

> **PIC16F877A-Based Industrial Proximity Sensing, Data Logging & Dual Communication (RS-232 / Wi-Fi) System**

RangeGuard is an industrial-grade embedded monitoring system designed for accurate non-contact distance measurement, real-time alerting, offline data logging, and dual communication through **RS-232** or **Wi-Fi**. It is built around the **PIC16F877A** microcontroller and was developed for the **PCB Hackathon 2026**.

---

## 📌 Project Overview

Industrial environments require reliable systems to monitor object proximity, trigger alarms, and record events without relying on a computer. RangeGuard provides an all-in-one solution by combining:

- Accurate laser-based distance sensing
- On-board data logging
- Industrial serial communication
- Wireless IoT connectivity
- Audible alert system
- 24V industrial power compatibility

---

## 🎯 Applications

- Industrial Safety Monitoring
- Machine Enclosures
- Conveyor Belt Monitoring
- Factory Automation
- Production Line Inspection
- Warehouse Object Detection
- Industrial IoT Systems
- Smart Manufacturing

---

## 🚀 Features

- 📏 Millimeter-accurate laser distance measurement
- 💾 Offline logging to microSD card
- 🔔 Buzzer alarm when threshold is crossed
- 🔄 Dual communication:
  - RS-232
  - Wi-Fi (ESP8266)
- ⚡ 24V industrial power input
- 📡 MQTT/HTTP compatible
- 🔧 Industrial-grade PCB design
- 🛡 EMC/EMI protection techniques implemented

---

## 🏗 System Architecture

<img width="838" height="552" alt="image" src="https://github.com/user-attachments/assets/7924c54d-f5a2-49d2-889b-c2889c8f8ee3" />

---
## 📐 Complete Schematic
  The complete schematic designed in Altium Designer, integrating the power supply, sensing, communication, and alert modules into a single industrial embedded system.

<img width="936" height="621" alt="image" src="https://github.com/user-attachments/assets/0bbc5b62-927c-453b-a885-ba2928f49bd7" />

---

## 🔷 PCB Top Layer
  Top layer showing component placement, signal routing, and optimized trace layout for reliable operation.
  <img width="931" height="394" alt="image" src="https://github.com/user-attachments/assets/77ad07f1-fe6f-4840-ab78-8a553868cde4" />

---
## 🔶 PCB Bottom Layer
  Bottom layer with a continuous ground plane to improve EMC performance and reduce return-path impedance.
  <img width="935" height="391" alt="image" src="https://github.com/user-attachments/assets/2efe09c0-a673-4b90-8578-22d7c030e9df" />
---
##  🖥️ 3D PCB View
  3D rendered view of the completed PCB illustrating the final component placement and mechanical layout.
  <img width="925" height="385" alt="image" src="https://github.com/user-attachments/assets/80dd6b00-2f07-4708-a0a3-a74fe0c7f473" />
## 🧩 Hardware Components

| Component | Purpose |
|------------|---------|
| PIC16F877A | Main Controller |
| VL53L0X | Laser Time-of-Flight Distance Sensor |
| TPS5403DR | 24V to 3.3V Buck Converter |
| MAX3232 | RS-232 Level Converter |
| ESP8266EX | Wi-Fi Communication |
| microSD Card | Data Logging |
| Piezo Buzzer | Audible Alert |
| DPDT Switch | Select RS-232 or Wi-Fi |

---

## ⚙ Working Principle

1. 24V industrial supply powers the system.
2. Buck converter regulates voltage to 3.3V.
3. PIC initializes all peripherals.
4. VL53L0X continuously measures distance.
5. PIC compares measured distance with preset threshold.
6. If threshold is crossed:
   - Buzzer is activated.
   - Reading is logged to microSD.
   - Data is transmitted through either:
     - RS-232
     - Wi-Fi (MQTT/HTTP)
7. System continues monitoring in real time.

---

## 📡 Communication Modes

### RS-232 Mode

- Industrial serial communication
- PC connectivity
- PLC integration
- HMI compatibility

### Wi-Fi Mode

- ESP8266 UART Interface
- MQTT Publishing
- HTTP Communication
- IoT Cloud Integration

---

## 💾 Data Logging

Sensor readings are stored in CSV format:

```csv
Timestamp,Distance(mm),Alarm
12:45:10,312,OFF
12:45:12,198,ON
12:45:14,195,ON
````

---

## 🔧 Protection Features

* Input Fuse Protection
* Schottky Protection Diode
* Flyback Diode
* Soft Start
* Decoupling Capacitors
* Ground Plane
* UART Isolation using DPDT Switch
* EMC/EMI Optimized PCB Layout

---

## 📋 Bill of Materials

* PIC16F877A
* VL53L0X
* ESP8266EX
* TPS5403DR
* MAX3232
* microSD Card Socket
* Piezo Buzzer
* DPDT Switch
* 8 MHz Crystal
* 82 µH Inductor
* Schottky Diode
* NPN Transistor
* Ceramic & Electrolytic Capacitors
* Resistors

---

## 📂 Repository Structure

```
RangeGuard/
│
├── Hardware/
│   ├── Schematic/
│   ├── PCB/
│   └── Gerber/
│
├── Firmware/
│   ├── PIC16F877A/
│   ├── ESP8266/
│   └── Libraries/
│
├── Images/
│   ├── PCB/
│   ├── 3D/
│   └── BlockDiagram/
│
├── Documentation/
│   └── Project_Report.pdf
│
└── README.md
```

---

## 🛠 Software & Tools

* Altium Designer
* GitHub

---

## 📈 Future Improvements

* OLED Display Interface
* GSM Alerts
* LoRa Communication
* Mobile Application
* OTA Firmware Updates
* Multiple Sensor Support
* Cloud Dashboard
* Predictive Maintenance Analytics

---

## 👨‍💻 Team

**Team Sentinels**

* **Sri Sanjai A** – Electronics and Communication Engineering
* **Vinith M K** – Electrical and Electronics Engineering

**Institution**

Bannari Amman Institute of Technology

---

## 📜 License

This project was developed as part of the **PCB Hackathon 2026**.

Feel free to use this repository for educational and research purposes.

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub!
