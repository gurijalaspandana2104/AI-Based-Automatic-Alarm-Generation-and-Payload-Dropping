# 🚁 AI-Based Disaster Management Drone

An **AI-powered autonomous drone system** designed for **disaster management and rescue operations**.  
This project combines **Computer Vision**, **IoT**, and **autonomous navigation** to detect humans, deliver payloads (like medical kits), and assist in rescue missions during natural disasters such as floods or earthquakes.

---

## 💡 Project Overview

During disasters, access to affected areas is often limited.  
This drone system provides **real-time detection and response** using **AI and sensors** — identifying humans in need, determining safe drop zones, and autonomously delivering relief payloads.

The system uses **YOLO-based object detection** for identifying humans and **DroneKit SDK** for flight control and mission execution, integrated with **LiDAR/ToF sensors** for accurate altitude and terrain detection.

---

## 🧩 Key Features

### 👁️ Human Detection using YOLO
- Integrated **YOLOv5/YOLOv7** for real-time object (human) detection.
- Runs inference using **Jetson Xavier NX / Jetson Nano** for edge AI computation.
- Capable of detecting humans in complex terrains and lighting conditions.

### 📦 Payload Delivery Mechanism
- Custom payload drop module triggered automatically after detection confirmation.
- Ensures safe release using altitude and object distance feedback from sensors.

### 📡 Autonomous Navigation
- Controlled via **DroneKit-Python SDK** and **ArduPilot** flight controller (Pixhawk).
- Supports **waypoint missions**, **RTL (Return-to-Launch)**, and **failsafe operations**.
- Real-time telemetry (altitude, GPS, battery) available on ground station.

### 🌍 Sensor Integration
- **LiDAR / ToF Laser Sensor:** Measures altitude with centimeter-level precision.  
- **GPS Module:** For navigation and positional accuracy.  
- **Camera Module:** For visual detection and live streaming.

### 🧠 AI and Control System
- **AI:** YOLO model for human detection.
- **Control System:** Python + DroneKit to automate drone movements and payload actions.
- **Failsafe Algorithms:** Prevent crashes by maintaining minimum altitude and avoiding obstacles.

---

## 🧰 Tech Stack

| Category | Technologies / Tools Used |
|-----------|---------------------------|
| Programming Languages | Python |
| AI / CV | YOLOv5, YOLOv7, OpenCV |
| Drone SDK | DroneKit-Python |
| Sensors | LiDAR, ToF Laser, GPS, IMU, Camera |
| Hardware | Jetson Xavier NX / Jetson Nano, Pixhawk (ArduPilot), Raspberry Pi |
| Communication | MAVLink Protocol |
| Development Tools | Google Colab, Mission Planner, QGroundControl |

---

## ⚙️ System Workflow

1. **Drone takes off** and follows pre-set waypoints (autonomous mission).  
2. **Camera captures video feed** and sends it to the onboard AI system.  
3. **YOLO model detects humans** in real time.  
4. If a human is detected:
   - Drone hovers and confirms detection.
   - **Payload is dropped automatically** using the servo mechanism.  
5. **Altitude data** is continuously monitored by **LiDAR/ToF sensors** for accuracy.  
6. Drone returns to base after completing its mission (RTL).

---

## 🎯 Learning Outcomes

- Integrated **AI and IoT for real-world robotics** applications.  
- Learned **drone flight control and telemetry using DroneKit**.  
- Gained hands-on experience with **Jetson edge AI devices** and **sensor calibration**.  
- Developed understanding of **computer vision**, **autonomous navigation**, and **payload systems**.  
- Applied **Python automation and hardware interfacing** to solve real disaster management problems.

---

