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
| Arduino Mega                 | 1        |
| Hoverboard motors + ESC      | 2 (or 4) |
| HC-SR04 Ultrasonic Sensor    | 4–6      |
| Motor Driver (e.g., VESC)    | 2+       |
| 12–36V Li-ion Battery        | 1        |
| Power Regulation Circuit     | 1        |
| Robot Frame / Chassis        | 1        |
| Optional: Bluetooth Module   | 1        |
| 27 Inch Touch Screen         | 1        |
| DC-DC Buck Converter         | 1        |
| Neon Strips for backlight    | 1        |
| Inverter                     | 1        |
| Raspberry pi 4               | 1        |
| Aluminum Extrusion Profile1m | 4        |
| 3mm Stainless Steel Sheet    | 3        |

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
- ![image](https://github.com/user-attachments/assets/d0650c3c-c89f-4247-be8a-4fb0f88f37f3)


### 3. Recommendations

• I DO NOT RECOMMEND using 3D Printed Material in this project. You should us plastic or
fiber glass and there are multiple manufacturers in Egypt.
• Aluminum for the profiles would be light weight and suitable.
• I DO NOT RECOMMEND skipping steps or changing the steps order each step is important to
be taken one at a time.
• Each step reveals a new modification in the design and the internal structure so be patient.
• You have to be flexible with components but never compensate in the material or the
structure.
• The design needs modifications for Neon Inserts and air cooling.
• The use of a fan for cooling should be studied.
• The timeline is always flexible.
• Modify the wheel plates for the project.
• Try to create new supports for body fixation with the robot.
• Make space for the cooling fans.

### 4. Install Dependencies
```bash
sudo apt update
sudo apt install python3-pip
pip3 install rpi.gpio numpy
# For SLAM:
# sudo apt install ros-<distro>-gmapping (if using ROS)


