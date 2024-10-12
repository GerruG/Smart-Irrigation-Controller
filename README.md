# Smart Irrigation Controller 🌱💧
A secure, IoT-based system for automating irrigation using an ESP32 microcontroller, sensors, and a web/mobile interface. Designed to optimize water usage and monitor soil conditions in real-time.

---

## Table of Contents
- [Overview](#overview)
- [System Architecture](#system-architecture)
- [Hardware Requirements](#hardware-requirements)
- [Software Setup](#software-setup)
- [Security](#security)
- [User Guide](#user-guide)
- [Future Enhancements](#future-enhancements)
- [License](#license)

---

## Overview
The **Smart Irrigation Controller** is an IoT project designed to automate and monitor irrigation systems with real-time data logging. It uses the **ESP32** microcontroller with various sensors to track soil moisture, temperature, and light levels. 

**Features:**
- Real-time monitoring and control
- Web Dashboard and Mobile App built with React
- Secure communication via Netbird VPN
- Data logging and historical analysis

![System Architecture](link-to-image) <!-- Replace with actual image link -->

---

## System Architecture
The system comprises the following components:
1. **ESP32 Microcontroller**: Handles sensor data and controls the water pump.
2. **Raspberry Pi Server**: Hosts backend services and serves the UI.
3. **Sensors**: Soil moisture, temperature, and light sensors.
4. **Actuator**: Water pump controlled via relay module.

Here's a high-level diagram of the system:

![System Diagram](link-to-image) <!-- Replace with actual image link -->

---

## Hardware Requirements
| Component               | Description                                      | Cost        |
|-------------------------|--------------------------------------------------|-------------|
| ESP32 Development Board | Wi-Fi-enabled microcontroller                    | $5 - $10    |
| Soil Moisture Sensor    | Resistive sensor for soil moisture detection     | $2 - $5     |
| Temperature Sensor      | DHT22 or DS18B20                                 | $3 - $5     |
| Light Sensor            | BH1750 or LDR                                    | $2 - $5     |
| Mini Water Pump         | Low-voltage DC pump                              | $5 - $10    |
| Relay Module            | Controls water pump with ESP32                   | $1 - $3     |
| Raspberry Pi            | Acts as the local server and VPN endpoint        | $35 - $75   |

---

## Software Setup
### Zephyr RTOS on ESP32
1. Install the Zephyr SDK.
2. Configure the networking stack for Wi-Fi connectivity.
3. Implement sensor drivers and control logic.

### Raspberry Pi Server
- Install Docker and Docker Compose.
- Set up Netbird VPN for secure communication.
- Develop backend with your preferred language and frameworks.

For detailed setup, see the [Software Guide](link-to-software-guide).

---

## Security
This project uses **Netbird VPN** for secure communication between the ESP32 and Raspberry Pi. 
- Ensure all data transmission occurs over VPN for encryption.
- API endpoints are secured with token-based authentication.

---

## User Guide
1. **Access the Dashboard**: View sensor data and control the water pump manually.
2. **Mobile App**: Install the React Native app for remote access on mobile devices.

### Dashboard Screenshot
![Dashboard Screenshot](link-to-image) <!-- Replace with actual image link -->

---

## Future Enhancements
- **Additional Sensors**: Add sensors like humidity or rain gauge for more accurate monitoring.
- **Cloud Integration**: Integrate with cloud services for remote monitoring and control.
- **Automated Notifications**: Send alerts for low soil moisture or pump activation.

---

## License
This project is licensed under the MIT License. See the [LICENSE](link-to-license) file for details.

---

