# RoboticArm
A custom-built 6-axis robotic arm powered by an ESP32 microcontroller, designed for real-time control via a web dashboard and integrated with ROS2 for advanced robotics applications. This project combines embedded systems, kinematics, and modern web-based control interfaces for a modular and extensible robotic solution.

---

## 🔧 Features

- 6 Degrees of Freedom using NEMA stepper motors
- ESP32 microcontroller with Wi-Fi for wireless control
- Real-time control interface through web dashboard
- MQTT protocol for low-latency communication
- Integration with ROS2 for simulation and autonomous behavior
- Modular design with customizable joints and links
- Future-ready for voice control (Google Assistant) and computer vision

---

## 🧱 Architecture

[Web UI] <--> [ESP32] <--> [Stepper Drivers] <--> [Robotic Arm]
| |
[MQTT Broker] <--> [ROS2 Node (Optional)]


---

## 📦 Tech Stack

- **Microcontroller:** ESP32 (WiFi-enabled)
- **Motion Control:** A4988/TMC2209 Stepper Drivers
- **Software:** Arduino IDE, PlatformIO
- **Control Interface:** HTML/CSS/JS + WebSocket/MQTT
- **Robotics Framework:** ROS2 (Foxy/Humble)
- **Simulation Tools:** RViz, MoveIt, Gazebo (optional)
- **Hardware Modeling:** SolidWorks & STL files for 3D printing

---

## 📂 Folder Structure

RoboticArm/
│
├── firmware/ # Arduino/ESP32 code
├── web-dashboard/ # Web UI for manual control
├── ros2_ws/ # ROS2 nodes and interfaces
├── hardware/ # CAD files and STL models
├── docs/ # Diagrams and documentation
└── README.md


---

## 🚀 Getting Started

1. **Hardware Setup**
   - Connect 6 stepper motors to ESP32 via drivers
   - Calibrate limit switches and power supply
   - Assemble arm using provided STL files

2. **Software Setup**
   - Flash firmware to ESP32 (via PlatformIO or Arduino IDE)
   - Open the Web UI and connect to MQTT broker
   - Launch ROS2 nodes (optional)

3. **Control Modes**
   - Manual: Web dashboard
   - Remote: MQTT messages
   - Autonomous: ROS2 planning stack

---

## 🎯 Use Cases

- Educational robotics platform
- Pick-and-place automation demos
- Integration testing with computer vision
- Research in path planning and ML-based motion control

---

## 📸 Preview

![Robotic Arm CAD](docs/cad-preview.png)  
*3D CAD model preview created in SolidWorks*

---

## 🛡 License

MIT License – feel free to use, modify, and contribute!

---
