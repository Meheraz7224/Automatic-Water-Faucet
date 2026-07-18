# Automatic Water Faucet

A low-power, touchless automatic water faucet system designed for hygienic operation and efficient water usage. The project uses an ESP32 microcontroller, infrared hand detection, and a latching solenoid valve to provide contactless water flow control while minimizing power consumption.

---

## 📌 Project Overview

This project aims to develop an energy-efficient automatic faucet suitable for washrooms, laboratories, and ablution (Wudhu) systems. The system detects the presence of a user's hand using an infrared sensing mechanism and activates a latching solenoid valve to control water flow.

Key objectives:

* Reduce water wastage
* Improve hygiene through touchless operation
* Minimize power consumption
* Enable future energy harvesting integration

---

## ✨ Features

* Touchless hand detection
* ESP32-based control system
* Low-power infrared sensing
* Latching solenoid valve control
* Current and power monitoring using INA219
* Ambient light compensation
* Adjustable detection range
* Fast response time
* Water-saving operation

---

## 🛠 Hardware Components

| Component       | Model                            |
| --------------- | -------------------------------- |
| Microcontroller | ESP32-WROOM-32                   |
| IR Emitter      | TSAL620                          |
| IR Receiver     | BPW34 / Photodiode               |
| Motor Driver    | DRV8833                          |
| Current Sensor  | INA219                           |
| Valve           | DC Latching Solenoid Valve       |
| Power Source    | Li-ion Battery / External Supply |

---

## 🏗 System Architecture

```text
Hand Detection
      │
      ▼
IR Sensor (TSAL620 + BPW34)
      │
      ▼
ESP32 Controller
      │
      ▼
DRV8833 Driver
      │
      ▼
Latching Solenoid Valve
      │
      ▼
Water Flow Control
```

---

## ⚙ Working Principle

1. The IR emitter continuously sends infrared light.
2. Reflected light from a hand is detected by the photodiode.
3. The ESP32 processes the sensor data.
4. When a valid hand is detected, the ESP32 activates the DRV8833 driver.
5. The driver sends a pulse to the latching solenoid valve.
6. Water flow starts.
7. After the hand is removed or a timeout occurs, the valve closes.

---

## 📂 Repository Structure

```text
Automatic-Water-Faucet
│
├── docs/
├── firmware/
├── hardware/
├── images/
├── results/
├── test/
├── videos/
└── README.md
```

---

## 📊 Performance

| Parameter        | Value               |
| ---------------- | ------------------- |
| Detection Method | Infrared Reflection |
| Detection Range  | 5–10 cm             |
| Response Time    | < 500 ms            |
| Valve Type       | Latching Solenoid   |
| Controller       | ESP32               |
| Power Monitoring | INA219              |

---

## 📸 Project Images

### Prototype

Add project photos here.

```markdown
![Prototype](images/prototype/prototype_front.jpg)
```

### Block Diagram

```markdown
![Block Diagram](images/diagrams/system_block_diagram.png)
```

### Schematic

```markdown
![Schematic](images/hardware/schematic.png)
```

### Experimental Results

```markdown
![Current Consumption](images/graphs/current_consumption.png)
```

---

## 🔬 Future Improvements

* Deep sleep implementation
* Improved ambient light rejection
* Energy harvesting integration
* PCB miniaturization
* Adaptive sensing algorithm
* Wireless monitoring

---

## 🎓 Academic Information

**Project Title:** Automatic Water Faucet Using Infrared Sensing and Low-Power Control

**Department:** Electrical and Electronic Engineering (EEE)

**University:** University of Chittagong

---

## 📜 License



---

## 📬 Contact

**Meheraz Rifat**

Electrical and Electronic Engineering Student

University of Chittagong

GitHub: https://github.com/YourUsername
