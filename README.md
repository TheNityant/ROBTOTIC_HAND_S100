# 🤖 Robotic Servo Control Projects

<p align="center">
  <strong>STM32-based servo control experiments and robotic mechanism prototypes developed using embedded C, UART communication, and controller-based interfaces.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/STM32F103-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="STM32F103"/>
  <img src="https://img.shields.io/badge/STM32F4-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="STM32F4"/>
  <img src="https://img.shields.io/badge/STM32CubeIDE-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="STM32CubeIDE"/>
  <img src="https://img.shields.io/badge/Embedded_C-00599C?style=flat-square&logo=c&logoColor=white" alt="Embedded C"/>
</p>

---

## 🎥 Demonstration

<p align="center">
  <a href="YOUR_YOUTUBE_URL">
    <img src="YOUR_VIDEO_THUMBNAIL_URL"
         width="800"
         alt="Robotic Servo Control Demonstration">
  </a>
</p>

<p align="center">
  <i>Demonstration of servo control and robotic mechanism operation.</i>
</p>

---

## 🧭 Overview

This repository contains a collection of STM32-based servo and motor-control projects developed while experimenting with embedded robotics and mechanism control.

The projects progress from basic UART-based servo control to multi-servo systems, PS4 controller interfaces, picking mechanisms, locomotion control, and servo-stepper integration.

The primary platforms used are **STM32F103** and **STM32F4**, with ESP-based controller interfaces used in several projects.

---

## 🧩 Projects

### 01 · SERVO_UART
**Single-servo control through UART**

A basic implementation for controlling a servo through UART communication. Serves as a starting point for experimenting with servo commands and embedded communication.

---

### 02 · MULTI_SERVO_UART
**Multi-servo control through UART**

Extends UART-based control to multiple servos with modular handling and STM32 HAL peripherals.

---

### 03 · PS4_SERVO_CONTROLLED
**PS4 controller → ESP receiver → STM32 → servo**

A controller-based servo control system using an ESP receiver to transmit PS4 controller input to the STM32.

---

### 04 · PS4_PICKING_MECHANISM_CONTROLLED
**PS4-controlled robotic picking mechanism**

A servo-control implementation developed for operating a robotic picking mechanism through a PS4 controller interface.

---

### 05 · SERVO_WORK_MODE
**Servo operating-mode experiments**

Experiments with different servo operating modes and motion patterns for embedded robotic applications.

---

### 06 · SERVO_STEPPER_INTEGRATION
**Servo + stepper motor integration**

Combines servo and stepper motor control within a single embedded system.

---

### 07 · PS4_SERVO_STEPPER_CTRL
**PS4-controlled servo and stepper system**

Integrates PS4 controller input with coordinated servo and stepper motor control.

---

### 08 · PS4_SERVO_STEPPER_LOCO_CONTROLLED
**Controller-based locomotion system**

A locomotion-oriented control implementation combining servo and stepper actuation with PS4 controller input.

---

### 09 · R1_PICKING_MECHANISM
**R1 robotic picking mechanism**

Control implementation developed around the R1 picking mechanism used in the robotics system.

---

### 10 · SERVO_ANGLE_CONTROL
**Servo positioning and angle control**

Experiments focused on precise servo positioning, angle control, and calibration.

---

### 11 · STM_F4
**STM32F4-based control experiments**

Embedded control projects developed on the STM32F4 platform, exploring the capabilities of a more powerful STM32 family compared with the STM32F103 projects.

---

## ⚙️ Technical Areas

### Embedded Control

- STM32F103
- STM32F4
- STM32 HAL
- STM32CubeIDE
- Embedded C
- UART communication
- Timer/peripheral configuration

### Motion Control

- Servo control
- Multi-servo coordination
- Servo positioning
- Stepper motor control
- Servo + stepper integration
- Robotic mechanism actuation

### Human-Machine Interfaces

- PS4 controller input
- ESP-based receiver interfaces
- UART-based communication between controllers and STM32

---

## 🔌 Typical Control Architecture

Several controller-based projects follow a structure similar to:

```text
      PS4 Controller
            │
            ▼
      ESP Receiver
            │
           UART
            │
            ▼
        STM32 MCU
            │
      ┌─────┴─────┐
      ▼           ▼
   Servos      Steppers
      │           │
      └─────┬─────┘
            ▼
      Robotic Mechanism
