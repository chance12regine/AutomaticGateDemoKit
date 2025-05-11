# 🚦 Ultrasonic Sensor Controlled Gate System

This Arduino project is an **automated gate control system** that detects nearby objects using an ultrasonic sensor and controls a servo motor to open or close a gate. It also provides visual (LED) and sound (buzzer) feedback for enhanced interactivity and safety.

## 🔧 Features

- **Object Detection** via HC-SR04 ultrasonic sensor.
- **Gate Automation** using a servo motor.
- **LED Indicators**:
  - 🔴 Red LED: Gate is closed.
  - 🔵 Blue LED: Gate is open.
- **Buzzer Alert** when an object is detected.
- **Auto-Close Function** after 5 seconds of no detection.

## 🛠 Hardware Components

- Arduino UNO
- HC-SR04 Ultrasonic Sensor
- Servo Motor (e.g., SG90)
- Red LED + Resistor
- Blue LED + Resistor
- Buzzer
- Jumper Wires
- Breadboard

## ⚙️ How It Works

1. Continuously measures distance using the ultrasonic sensor.
2. If an object is within 50 cm:
   - Gate opens.
   - Blue LED turns ON, Red LED turns OFF.
   - Buzzer activates.
3. If the object moves away and 5 seconds pass:
   - Gate closes.
   - Red LED turns ON, Blue LED turns OFF.
   - Buzzer deactivates.

## 📁 File

- `main.ino`: Main Arduino sketch with complete logic.

## 🧰 Setup Instructions

1. Connect all components as per the code pin definitions.
2. Upload the `main.ino` file to your Arduino board.
3. Power the board and observe the gate respond to nearby objects.

---

Feel free to contribute or fork this project to improve or adapt it for your own automation needs!
