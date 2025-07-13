# Dual ESC System – STM32L431-Based Motor Controller

This project presents a dual Electronic Speed Controller (ESC) system designed around the STM32L431KC microcontroller. Each ESC channel is capable of independently driving a three-phase brushless motor, with integrated current sensing, voltage monitoring, and dedicated gate drivers for precise and reliable motor control.

---

## 📘 Overview

The design includes two identical ESC channels. Each channel consists of:

- **STM32L431KC Microcontroller**  
  Responsible for control logic, PWM generation, and real-time processing of feedback data.

- **FD6288 Gate Driver**  
  High-speed 3-phase driver IC for controlling the motor power MOSFETs.

- **Phase Outputs (A, B, C)**  
  Three-phase half-bridge outputs connected to the brushless motor.

- **Current Sense Circuit**  
  Provides phase current feedback for protection and closed-loop control.

- **Voltage & Current Monitor**  
  Supplies operating feedback to the MCU for performance tuning and fault detection.

- **Motor Pad**  
  Terminal block for connecting each brushless DC motor.

- **Battery Pad**  
  Power input terminal for each ESC unit.

Each ESC also includes a dedicated **SWD (Serial Wire Debug)** interface for firmware programming and debugging.

---

## 🔋 Power Section

The system includes onboard voltage regulation for multiple power domains:

- **3.3V** – Logic supply for MCU and sensors  
- **5V** – Peripherals and I/O  
- **8.4V** – Intermediate voltage rail  
- **12V** – Power stage / gate drive circuitry

Power rails are isolated and filtered to ensure stability and to protect control logic from switching noise introduced by the motor stages.

---

## 🛠️ Applications

This dual ESC design is suitable for a range of multi-motor embedded control systems, including:

- 🚁 Multirotor drones and UAVs  
- 🤖 Robotics and automation platforms  
- 🚗 Electric vehicles and mobility systems  
- ⚙️ Industrial multi-axis motor control

---

## 📂 Included Files

- ✅ Full schematic design (`.sch` – KiCad format)  
- ✅ Block-level system diagram  
- ✅ Subsystem functional documentation  

---

## 👨‍💻 Author

**Muddessir Arif**  
📞 +92 340 0586446  
📧 [muddessirarif140174@gmail.com](mailto:muddessirarif140174@gmail.com)

---

> ⚠️ This project is intended for development, education, and prototyping. Use with proper electrical safety precautions when working with power electronics and brushless motors.
