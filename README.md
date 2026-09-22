# 🤖 Robotis — Smart Bluetooth-Controlled Robot.

Robotis is an Arduino-based smart robotic system that can be controlled wirelessly through a mobile application. The robot combines **Bluetooth-based control, obstacle detection, and environmental monitoring** into a single embedded system.

The project was developed to explore **Arduino programming, sensors, motor control, Bluetooth communication, and mobile-app-based robotics**.

## 🚀 Features

* 📱 **Bluetooth Control** — Control the robot wirelessly using a mobile application.
* 🚗 **Motor Control** — Move the robot forward, backward, left, and right.
* 🛑 **Obstacle Detection** — Uses an ultrasonic sensor to detect nearby obstacles.
* 🌡️ **Temperature Monitoring** — Measures temperature using a DHT sensor.
* 💧 **Humidity Monitoring** — Measures surrounding humidity using a DHT sensor.
* 📲 **Mobile Application** — Built using MIT App Inventor.
* 🔌 **Arduino-Based Control** — Arduino handles sensors, motors, and communication.
* 📐 **Circuit Schematic** — Includes the complete hardware connection diagram.

## 🧠 System Overview

The system consists of three major components:

```text
                ┌──────────────────────┐
                │   Mobile Application │
                │    MIT App Inventor  │
                └──────────┬───────────┘
                           │
                       Bluetooth
                           │
                           ▼
                ┌──────────────────────┐
                │       Arduino        │
                │   Main Controller    │
                └──────┬───────┬───────┘
                       │       │
              ┌────────┘       └─────────┐
              ▼                          ▼
       ┌─────────────┐            ┌──────────────┐
       │ Motor Driver│            │    Sensors   │
       │   & Motors  │            │              │
       └─────────────┘            │ Ultrasonic   │
                                  │ DHT Sensor   │
                                  └──────────────┘
```

## 🛠️ Hardware Components

| Component         | Purpose                             |
| ----------------- | ----------------------------------- |
| Arduino           | Main microcontroller                |
| DC Motors         | Robot movement                      |
| Motor Driver      | Controls motor direction and speed  |
| Bluetooth Module  | Wireless communication              |
| Ultrasonic Sensor | Obstacle detection                  |
| DHT Sensor        | Temperature and humidity monitoring |
| Robot Chassis     | Mechanical structure                |
| Battery           | Power supply                        |
| Connecting Wires  | Circuit connections                 |

## 💻 Software & Technologies

* **Arduino / Embedded C++**
* **MIT App Inventor**
* **Bluetooth Communication**
* **Ultrasonic Sensor**
* **DHT Sensor**
* **Embedded Systems**
* **Motor Control**

## 📁 Project Structure

```text
Robotis/
│
├── project_robot.ino       # Main Arduino program
├── dht.cpp                  # DHT sensor implementation
├── dht.h                    # DHT sensor header
├── project_robot.aia        # MIT App Inventor project
├── Schematic_robot.pdf      # Hardware circuit schematic
└── README.md                # Project documentation
```

## ⚙️ How It Works

### 1. Mobile Control

The mobile application sends movement commands to the robot through Bluetooth.

Example commands include:

```text
Forward
Backward
Left
Right
Stop
```

### 2. Arduino Processing

The Arduino receives Bluetooth commands and converts them into motor-control signals.

### 3. Obstacle Detection

The ultrasonic sensor continuously measures the distance between the robot and nearby objects.

If an obstacle is detected within a defined range, the robot can respond accordingly.

### 4. Environmental Monitoring

The DHT sensor collects:

* Temperature
* Humidity

These values can be processed by the Arduino and used by the application/system.

## 📱 Mobile Application

The mobile application was developed using **MIT App Inventor**.

The `.aia` project file is included in this repository so that the application can be imported and modified.

### Import the App

1. Open MIT App Inventor.
2. Go to **Projects**.
3. Select **Import project (.aia) from my computer**.
4. Select `project_robot.aia`.
5. Open and modify the application as required.

## 🔧 Setup

### Arduino

1. Install the Arduino IDE.
2. Connect the Arduino board to your computer.
3. Open:

```text
project_robot.ino
```

4. Install the required sensor libraries if needed.
5. Select the correct Arduino board and COM port.
6. Upload the program.

### Hardware

Connect the components according to:

```text
Schematic_robot.pdf
```

Make sure the motor driver, sensors, Bluetooth module, and power supply are connected correctly before powering the robot.

## ▶️ Running the Project

1. Upload the Arduino program.
2. Power on the robot.
3. Enable Bluetooth on the mobile device.
4. Open the Robotis mobile application.
5. Connect to the robot's Bluetooth module.
6. Use the controls to operate the robot.
7. Monitor sensor data where supported.

## 🎯 Learning Objectives

This project demonstrates practical understanding of:

* Embedded systems
* Arduino programming
* Sensor interfacing
* Bluetooth communication
* DC motor control
* Obstacle detection
* Temperature and humidity sensing
* Mobile-to-hardware communication
* Basic robotics

## 🔮 Future Improvements

Possible future enhancements include:

* 🤖 Autonomous navigation
* 🧠 AI-based obstacle avoidance
* 📍 GPS-based tracking
* 📷 Camera-based object detection
* 📊 Real-time sensor dashboard
* ☁️ IoT/cloud connectivity
* 🔋 Battery-level monitoring
* 🎙️ Voice-controlled navigation

## 📜 License

This project is intended for educational and learning purposes.

Third-party libraries or code included in the project remain subject to their respective licenses and original authorship.

## 👨‍💻 Author

**Syed Ayan Husain**

GitHub: [@syedayan990](https://github.com/syedayan990)
