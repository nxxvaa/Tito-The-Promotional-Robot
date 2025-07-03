# 🤖 Tito: The Open-Source Promotional Robot

> Innovation is meant to be shared — not stolen.

Tito is a mobile promotional robot designed for events, exhibitions, and interactive product showcases. Originally created by me, the design was unfortunately used without permission by a commercial entity. As a response, I’m making **Tito fully open-source** so anyone can build, modify, and deploy it freely.

---

## 🚀 What is Tito?

**Tito** is an autonomous, four-wheeled robot that uses:
- **Ultrasonic sensors** for real-time obstacle avoidance
- **SLAM (Simultaneous Localization and Mapping)** to generate maps of indoor spaces
- A **Raspberry Pi** for onboard control
- **Hoverboard motors** salvaged from standard boards for mobility and torque

Whether you’re showcasing products or demonstrating robotics, Tito makes your work stand out — literally and technically.

---

## 🧠 Key Features

- 🛑 **Obstacle Avoidance** with HC-SR04 ultrasonic sensors
- 🗺️ **Live Mapping** using lightweight SLAM algorithms
- 🧠 **Raspberry Pi-based** brain for control and logic
- 🛞 **Hoverboard wheels** for reliable, powerful drive
- 📦 **Modular Design** to attach promo screens, lighting, or giveaways

---

## 🔩 Hardware List

| Component                     | Quantity |
|------------------------------|----------|
| Raspberry Pi 4 / 3B+         | 1        |
| Hoverboard motors + ESC      | 2 (or 4) |
| HC-SR04 Ultrasonic Sensor    | 4–6      |
| Motor Driver (e.g., VESC)    | 2+       |
| 12–36V Li-ion Battery        | 1        |
| Power Regulation Circuit     | 1        |
| Robot Frame / Chassis        | 1        |
| Optional: LIDAR              | 1        |

---

## 🖥️ Software Stack

- **OS**: Raspberry Pi OS / Ubuntu
- **Language**: Python 3
- **Control**: GPIO + PWM
- **Mapping**: TinySLAM, GMapping (via ROS), or custom SLAM
- **Motor Control**: UART / PWM communication
- **Optional Web/Mobile UI** for monitoring and interaction

---

## ⚙️ Setup Instructions

### 1. Assemble the Chassis
- Mount the hoverboard wheels to a custom or metal frame.
- Secure the Pi, battery, and electronics.

### 2. Wire Up Components
- Connect ultrasonic sensors to GPIO pins.
- Connect ESCs to Pi and power distribution system.

### 3. Install Dependencies
```bash
sudo apt update
sudo apt install python3-pip
pip3 install rpi.gpio numpy
# For SLAM:
# sudo apt install ros-<distro>-gmapping (if using ROS)
