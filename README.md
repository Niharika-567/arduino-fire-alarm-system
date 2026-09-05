# arduino-fire-alarm-system
# 🔥 IoT-Based Fire Alarm System

An automated safety and early-warning system designed to monitor ambient temperature and hazardous gases in real-time using an Arduino Uno microcontroller[cite: 1].

---

## 🚀 Features
* **Dual Sensor Monitoring:** Continuously tracks environmental safety using both a temperature sensor (TMP36) and a gas sensor.
* **Automated Early Warnings:** Instantly triggers a piezo buzzer and an LED indicator when temperature or gas levels exceed predefined safety thresholds.
* **Microcontroller Logic:** Uses an Arduino Uno R3 as the primary processing unit running custom C++ logic.
* **Simulated & Prototyped:** Designed and tested using Tinkercad circuit simulation.

---

## 🛠️ Components Used
* **Microcontroller:** Arduino Uno R3
* **Sensors:** TMP36 Temperature Sensor, Gas Sensor 
* **Output Actuators:** Piezo Buzzer, Red LED with Resistors
* **Prototyping:** Small Breadboard and jumper wires

---

## ⚙️ How It Works
1. The sensors continuously read analog environmental data and send it to the Arduino Uno.
2. The system calculates temperature values and compares them against set limits (`tempThreshold = 50.0°C`, `gasThreshold = 300`).
3. If a hazard is detected, the system outputs an alert via the Serial Monitor (`!!! FIRE ALERT !!!`), lights up the LED, and sounds the buzzer.

---

## 💻 Code Snippet
You can find the full C++ implementation in the `fire_alarm.ino` (or main source file) within this repository, which handles pin configuration, threshold checks, and conditional alert triggers.
