# 🔥 Smart LPG Gas Leakage Detection & Automatic Shutoff System (ESP32)

## 📌 Project Overview

This project is a **Smart LPG Gas Leakage Detection and Automatic Shutoff System** built using **ESP32**.

The system detects gas leakage using an MQ-2 sensor and automatically:

* 🚨 Displays a warning on LCD
* 🔔 Activates a buzzer
* 🔄 Rotates a servo motor to turn OFF the gas regulator

This project improves household and industrial safety by preventing gas-related accidents.

---

## 🎯 Objectives

* Detect LPG gas leakage
* Provide visual and audible alert
* Automatically shut off gas supply
* Simulate the system using Wokwi
* Build a real-world safety prototype

---

## 🧩 Components Used

* ESP32
* MQ-2 Gas Sensor
* SG90 Servo Motor
* 16x2 LCD (I2C)
* Buzzer
* Connecting wires
* External 5V supply (for real hardware)

---

## 🔌 Circuit Connections

### MQ-2 Sensor

| MQ-2 Pin | ESP32 Pin |
| -------- | --------- |
| VCC      | 5V        |
| GND      | GND       |
| AO       | GPIO34    |
| DO       | Not used  |

---

### Servo Motor

| Servo Wire | ESP32 Pin |
| ---------- | --------- |
| Red        | 5V        |
| Brown      | GND       |
| Orange     | GPIO18    |

---

### LCD (I2C)

| LCD Pin | ESP32 Pin |
| ------- | --------- |
| VCC     | 5V        |
| GND     | GND       |
| SDA     | GPIO21    |
| SCL     | GPIO22    |

---

### Buzzer

| Buzzer | ESP32  |
| ------ | ------ |
| +      | GPIO23 |
| -      | GND    |

---

## ⚙️ Working Principle

1. The MQ-2 sensor continuously monitors gas concentration.
2. ESP32 reads the analog value from the sensor.
3. If gas level exceeds a predefined threshold:

   * LCD displays **"!!! GAS LEAK !!!"**
   * Buzzer turns ON
   * Servo rotates 90° to close gas regulator
4. If gas level is normal:

   * LCD displays **"System Safe"**
   * Buzzer OFF
   * Servo returns to normal position

---

## 🧪 Simulation in Wokwi

This project was simulated using **Wokwi ESP32 Simulator**.

### Steps to Test:

1. Start the simulation
2. Open Serial Monitor
3. Click on MQ-2 sensor
4. Increase the **Gas Level slider**
5. Observe:

   * LCD warning
   * Servo rotation
   * Buzzer activation

---

## 🛠️ Key Features

* Real-time gas monitoring
* Automatic regulator shutdown
* Audible and visual alert system
* Simulation-ready design
* Expandable IoT architecture

---

## 🚀 Future Enhancements

* 📲 WiFi alert notification (Blynk / Email / MQTT)
* 🌬 Automatic exhaust fan activation
* 🔋 Battery backup system
* 📊 Cloud data logging
* 🔒 Solenoid valve for industrial-grade control
* 📱 Mobile application interface

---

## ⚠️ Safety Note

For real hardware implementation:

* Use a high-torque servo motor
* Ensure proper mechanical mounting
* Use an external power supply for servo
* Test carefully in controlled environments

---

## 🎓 Learning Outcomes

* ESP32 ADC interfacing
* Sensor threshold calibration
* Actuator control (Servo)
* I2C communication (LCD)
* Embedded system design
* Safety system implementation

---

## 👨‍💻 Author

Developed as an IoT-based safety system project using ESP32.

---

⭐ If you found this project useful, consider starring the repository!
