# ✈️ Hybrid Fixed-Wing VTOL UAV

<p align="center">
  <h2 align="center">Development of a Hybrid Fixed Wing Drone (VTOL)</h2>
</p>

<p align="center">
  <b>Hybrid UAV • Fixed-Wing • VTOL • Embedded Systems • Flight Control</b>
</p>

<p align="center">
  <img width="375" height="381" alt="image" src="https://github.com/user-attachments/assets/62c7828a-3495-4aa3-8bf2-9ea376f47e2d" />

</p>

<p align="center">
  <i>A student-developed hybrid fixed-wing VTOL UAV prototype for surveillance-oriented applications.</i>
</p>

---

## 📌 Overview

The **Hybrid Fixed-Wing VTOL UAV** project focuses on the development of a fixed-wing unmanned aerial vehicle incorporating vertical take-off and landing capability.

The project combines the aerodynamic advantages of fixed-wing flight with the operational flexibility of VTOL configuration.

### Project Highlights

- **Airframe:** Hybrid fixed-wing VTOL UAV
- **Primary Application:** Aerial surveillance
- **Flight Controller:** SpeedyBee F405 Wing
- **MCU:** STM32F405, 32-bit ARM Cortex-M4
- **Propulsion:** 1200 KV brushless motor
- **ESC:** 40 A Electronic Speed Controller
- **RC System:** FlySky FS-i6S transmitter + FS-iA10B receiver
- **Airframe Material:** 5 mm foam board
- **3D Printing Materials:** PETG and LW-PLA
- **CAD Software:** FreeCAD
- **Configuration Software:** Mission Planner / Configurator
- **Project Type:** Student Innovative Project
- **Current Status:** Prototype / Proof of Concept

---

# 🎯 Objectives

The major objectives of the project are:

- Design an aerodynamic and lightweight fixed-wing UAV.
- Develop a hybrid VTOL configuration for vertical take-off and landing.
- Integrate the SpeedyBee F405 Wing flight controller.
- Configure and calibrate the flight-controller sensors.
- Implement RC transmitter and receiver communication.
- Configure the motor and ESC system.
- Perform propulsion and thrust testing.
- Conduct practical ground and flight testing.
- Identify prototype limitations and possible improvements.

---

# 👥 Team & Contributors


- **Vishal R**
- **Harishwar A**
- **Surya M**


---

# 🔧 Hardware Components

<table align="center">
  <thead>
    <tr>
      <th align="center">Component</th>
      <th align="center">Purpose</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>SpeedyBee F405 Wing</strong></td>
      <td align="center">Main flight controller</td>
    </tr>
    <tr>
      <td align="center"><strong>STM32F405 MCU</strong></td>
      <td align="center">Flight-control processing</td>
    </tr>
    <tr>
      <td align="center"><strong>Gyroscope</strong></td>
      <td align="center">Motion and angular-rate sensing</td>
    </tr>
    <tr>
      <td align="center"><strong>Accelerometer</strong></td>
      <td align="center">Motion sensing and stabilization</td>
    </tr>
    <tr>
      <td align="center"><strong>BMP280 Barometer</strong></td>
      <td align="center">Altitude sensing</td>
    </tr>
    <tr>
      <td align="center"><strong>1200 KV Brushless Motor</strong></td>
      <td align="center">Aircraft propulsion</td>
    </tr>
    <tr>
      <td align="center"><strong>40 A ESC</strong></td>
      <td align="center">Motor speed control</td>
    </tr>
    <tr>
      <td align="center"><strong>FlySky FS-i6S</strong></td>
      <td align="center">RC transmitter</td>
    </tr>
    <tr>
      <td align="center"><strong>FlySky FS-iA10B</strong></td>
      <td align="center">RC receiver</td>
    </tr>
    <tr>
      <td align="center"><strong>Servo Motors</strong></td>
      <td align="center">Control and actuation</td>
    </tr>
    <tr>
      <td align="center"><strong>5 mm Foam Board</strong></td>
      <td align="center">Airframe construction</td>
    </tr>
    <tr>
      <td align="center"><strong>PETG</strong></td>
      <td align="center">Structural 3D-printed parts</td>
    </tr>
    <tr>
      <td align="center"><strong>LW-PLA</strong></td>
      <td align="center">Lightweight aerodynamic parts</td>
    </tr>
    <tr>
      <td align="center"><strong>LiPo Battery</strong></td>
      <td align="center">Primary power source</td>
    </tr>
  </tbody>
</table>

---

# ⚙️ SpeedyBee F405 Wing Flight Controller

The **SpeedyBee F405 Wing** is used as the primary flight controller of the UAV prototype.

<p align="center">
  <img width="362" height="409" alt="image" src="https://github.com/user-attachments/assets/696bce03-c98e-485a-9704-0795f520ef84" />

</p>

## Specifications

<table align="center">
  <thead>
    <tr>
      <th align="center">Category</th>
      <th align="center">Specification</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Processor (MCU)</strong></td>
      <td align="center">STM32F405, 32-bit ARM Cortex-M4, 168 MHz</td>
    </tr>
    <tr>
      <td align="center"><strong>IMU (Gyro &amp; Accel)</strong></td>
      <td align="center">ICM-42688-P or MPU6000 (depends on batch)</td>
    </tr>
    <tr>
      <td align="center"><strong>Barometer</strong></td>
      <td align="center">BMP280 (for altitude sensing)</td>
    </tr>
    <tr>
      <td align="center"><strong>Flash Memory</strong></td>
      <td align="center">16MB onboard Blackbox data logging</td>
    </tr>
    <tr>
      <td align="center"><strong>UART Ports</strong></td>
      <td align="center">6 total – for GPS, telemetry, RC receiver, airspeed, etc.</td>
    </tr>
    <tr>
      <td align="center"><strong>I2C Port</strong></td>
      <td align="center">1 I2C port – for external sensors like airspeed sensor</td>
    </tr>
    <tr>
      <td align="center"><strong>PWM Outputs</strong></td>
      <td align="center">9 outputs – for ESCs, servos, and VTOL motors</td>
    </tr>
    <tr>
      <td align="center"><strong>Input Voltage</strong></td>
      <td align="center">7V – 35V (Supports 2S to 8S LiPo)</td>
    </tr>
    <tr>
      <td align="center"><strong>BEC Output</strong></td>
      <td align="center">5V/3A and 9V/2A for powering external devices</td>
    </tr>
    <tr>
      <td align="center"><strong>Wireless Configuration</strong></td>
      <td align="center">Built-in Wi-Fi and Bluetooth via SpeedyBee App</td>
    </tr>
    <tr>
      <td align="center"><strong>Firmware Compatibility</strong></td>
      <td align="center">INAV, ArduPilot</td>
    </tr>
    <tr>
      <td align="center"><strong>Telemetry Protocols</strong></td>
      <td align="center">FrSky SmartPort, FPort, SBUS, CRSF, ELRS, MAVLink</td>
    </tr>
    <tr>
      <td align="center"><strong>OSD Support</strong></td>
      <td align="center">Yes – analog OSD supported</td>
    </tr>
    <tr>
      <td align="center"><strong>Current Sensor</strong></td>
      <td align="center">Integrated analog sensor, supports up to 100A</td>
    </tr>
    <tr>
      <td align="center"><strong>Mounting Dimensions</strong></td>
      <td align="center">30.5mm × 30.5mm, standard M3 hole spacing</td>
    </tr>
    <tr>
      <td align="center"><strong>Board Dimensions</strong></td>
      <td align="center">~37mm × 37mm, excluding connectors</td>
    </tr>
    <tr>
      <td align="center"><strong>Weight</strong></td>
      <td align="center">Approx. 10 grams</td>
    </tr>
  </tbody>
</table>

---

# 🛩️ Airframe Design

The UAV uses a hybrid fixed-wing configuration designed to combine fixed-wing flight with VTOL capability.

<p align="center">
  <img width="765" height="432" alt="image" src="https://github.com/user-attachments/assets/f0efa75d-dafc-4c8d-8f9f-382deada99cb" />

</p>

## Main Design Features

- Fixed-wing aerodynamic structure
- Vertical-lift propulsion
- Rear-mounted pusher motor
- V-tail configuration
- Streamlined fuselage
- Lightweight construction
- Modular structural components
- 3D-printed components

---

# 📐 3D Modelling & CAD Design

The aircraft design was developed using **FreeCAD**.

<p align="center">
 <img width="674" height="458" alt="image" src="https://github.com/user-attachments/assets/984845e4-0cd7-40d0-9bf6-ffffaceb7a2f" />

</p>

## Design Materials

- **5 mm Foam Board** – lightweight airframe construction
- **PETG** – structural and higher-stress components
- **LW-PLA** – lightweight aerodynamic components

---

## ⚖️ License

This project is released under a **Custom License**. See [LICENSE](LICENSE) for full terms.

Public viewing is allowed, but **forking and reuse require prior permission**.

