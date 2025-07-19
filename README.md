# 🚗 Line Following Robot using 8051 Microcontroller

## 📌 Project Overview
This project focuses on designing and implementing a **Line Following Robot** using the **8051 microcontroller**. It is an autonomous robot capable of following a predefined path, usually a black line on a white surface or vice versa, using **IR sensors** and basic embedded programming. 

The objective is to explore embedded system concepts, sensor interfacing, and real-time motor control for simple robotics.

---

## 📝 Abstract
The **Line Follower Robot** autonomously follows a marked path by using **infrared (IR) sensors** to detect the line. The **8051 microcontroller** processes signals from the sensors and controls the motors through a motor driver module to adjust the direction. This project integrates both **hardware and software components** for real-time decision-making in line tracking.

---

## 🛠️ Components Required

| Component                          | Purpose / Description                                               |
|-------------------------------------|---------------------------------------------------------------------|
| **8051 Microcontroller (AT89S52)** | Core controller with I/O capabilities                               |
| **Development Board (8051)**       | Simplifies programming and testing with built-in support circuits   |
| **L298N Motor Driver Module**      | Drives two DC motors with external power support                    |
| **IR Sensors (2 units)**           | Detects black line by reflective light principles                   |
| **Robot Chassis**                  | Physical base with mounting for motors, sensors, and electronics    |
| **DC Motors (2 units)**            | Drives the robot wheels                                             |
| **Power Supply**                   | 12V battery and regulated 5V supply for microcontroller             |
| **Connecting Wires**               | For electrical connections                                          |

---

## ⚙️ Methodology

### 1. Sensor Section:
- **IR sensors** emit infrared light and detect reflection from the surface.
- **Comparator circuit (LM358)** converts analog IR sensor values into digital signals.
- Two comparator outputs (for left and right sensors) are fed to microcontroller **Port P0.0 and P0.1**.

### 2. Control Section:
- The **8051 microcontroller** receives sensor signals.
- Based on sensor input, it processes decisions and sends control signals to the motor driver via **Port P2**.

### 3. Driver Section:
- The **L298N Motor Driver** receives control signals and drives the two DC motors.
- Enables proper voltage/current to motors as 8051 cannot drive motors directly.

<img width="998" height="474" alt="image" src="https://github.com/user-attachments/assets/1ea8170c-2d38-4c2f-8697-4c67155bbe56" />


---

## ⚡ Working Principle

| Sensor Status                     | Robot Behavior        |
|-----------------------------------|------------------------|
| Left = 0, Right = 0               | Move **Forward**       |
| Left = 0, Right = 1               | Turn **Left**          |
| Left = 1, Right = 0               | Turn **Right**         |
| Left = 1, Right = 1               | **Stop**               |

- **0** → Sensor on black line (low reflection)
- **1** → Sensor on white surface (high reflection)

<img width="425" height="339" alt="image" src="https://github.com/user-attachments/assets/3b74ac8e-d7cd-4623-b8c8-989b04f7eb1d" />

<img width="423" height="329" alt="image" src="https://github.com/user-attachments/assets/0d7919f1-082b-4709-bfaa-3c3cd4832847" />

<img width="339" height="359" alt="image" src="https://github.com/user-attachments/assets/c9573389-0871-4dd6-9278-63e8b9af0e23" />

<img width="380" height="326" alt="image" src="https://github.com/user-attachments/assets/dfa3d794-8f89-4600-aa6a-47ea753be4ea" />

---
## Circuit Diagram

<img width="984" height="642" alt="image" src="https://github.com/user-attachments/assets/03011fd2-2325-4127-9974-c1887ed2add8" />

---

## ✅ Expected Outcomes
- Robot follows the **black line accurately**.
- **Real-time autonomous decision-making** with basic control logic.
- Basic introduction to **8051 programming**, **motor driving**, and **IR sensor interfacing**.

---

## 📊 Summary of Learning
- Gained **hands-on experience** in embedded systems, hardware interfacing, and basic robotics.
- Understood the application of **sensors, comparators, motor drivers**, and **microcontrollers** in real-world projects.
- Explored the concept of **real-time data processing** in autonomous robotic systems.

---

## 🎁 Conclusion
The **Line Following Robot** using the **8051 microcontroller** successfully demonstrates **autonomous navigation principles** using basic embedded system concepts. By integrating **IR sensors**, **L298N motor driver**, and **8051**, this project shows how **simple yet effective robotic solutions** can be designed with **fundamental electronics and programming knowledge**.


