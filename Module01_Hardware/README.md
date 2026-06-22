# Module 1: Introduction to Autonomous Vehicle Hardware and Connections

## Overview

In this module, students will learn the basic hardware components of an autonomous vehicle, understand their functions, assemble the NxGV vehicle kit, and verify that all components are working correctly.

---

## Learning Outcomes

By the end of this module, students should be able to:

- Identify the major hardware components of an autonomous vehicle.
- Explain the function of each component.
- Connect sensors and actuators to the ESP32 controller.
- Assemble the NxGV vehicle kit.
- Test each hardware component individually.

---

# Autonomous Vehicle Architecture

An autonomous vehicle consists of three major subsystems:

## 1. Perception

Perception allows the vehicle to sense its surroundings.

Examples:
- IR Sensors
- Ultrasonic Sensors
- Cameras
- LiDAR

---

## 2. Decision Making

The controller processes sensor information and decides what action to take.

Examples:
- ESP32
- Arduino
- Raspberry Pi

---

## 3. Actuation

Actuators perform physical actions based on the controller's commands.

Examples:
- DC Motor
- Servo Motor

---

# Hardware Components

## ESP32 Controller

The ESP32 acts as the brain of the autonomous vehicle.

Functions:
- Reads sensor data
- Processes information
- Controls motors and steering
- Executes autonomous algorithms

![ESP32](Images/esp32.jpg)

---

## DC Motor

The DC motor provides propulsion for the vehicle.

Functions:
- Move forward
- Move backward
- Speed control

![DC Motor](Images/dc_motor.jpg)

---

## Motor Driver

The motor driver allows the ESP32 to control the DC motor.

Functions:
- Motor direction control
- Motor speed control
- Current amplification

![Motor Driver](Images/motor_driver.jpg)

---

## Servo Motor

The servo motor controls vehicle steering.

Functions:
- Turn left
- Turn right
- Maintain steering angle

![Servo](Images/servo.jpg)

---

## IR Sensors

IR sensors detect the line on the track.

Functions:
- Line detection
- Navigation guidance

![IR Sensor](Images/ir_sensor.jpg)

---

## Ultrasonic Sensor

The ultrasonic sensor measures distance to nearby objects.

Functions:
- Obstacle detection
- Collision avoidance

![Ultrasonic](Images/ultrasonic.jpg)

---

# Hardware Connections

## ESP32 Pin Configuration

| Component | ESP32 Pin |
|------------|------------|
| Servo | GPIO 13 |
| Motor ENA | GPIO 5 |
| Motor IN1 | GPIO 18 |
| Motor IN2 | GPIO 19 |
| Ultrasonic TRIG | GPIO 27 |
| Ultrasonic ECHO | GPIO 14 |
| IR S1 | GPIO 25 |
| IR S2 | GPIO 33 |
| IR S3 | GPIO 32 |
| IR S4 | GPIO 35 |
| IR S5 | GPIO 34 |

---

## Wiring Diagram

![Wiring Diagram](Circuit_Diagrams/wiring_diagram.png)

---

# Practical Activity 1: Vehicle Assembly

### Objectives

- Assemble the vehicle chassis
- Install the DC motor
- Install the steering servo
- Mount all sensors
- Connect the battery

### Deliverable

A fully assembled autonomous vehicle.

---

# Practical Activity 2: Hardware Connections

### Objectives

- Connect all sensors
- Connect the motor driver
- Connect the steering servo
- Verify power supply wiring

### Deliverable

A correctly wired autonomous vehicle.

---

# Practical Activity 3: Hardware Testing

### Servo Test

Expected Outcome:
- Turn left
- Turn right
- Return to center

Code:
[Servo Test](Code/Servo_Test.ino)

---

### Motor Test

Expected Outcome:
- Move forward
- Stop

Code:
[Motor Test](Code/Motor_Test.ino)

---

### IR Sensor Test

Expected Outcome:
- Detect black and white surfaces

Code:
[IR Sensor Test](Code/IR_Test.ino)

---

### Ultrasonic Sensor Test

Expected Outcome:
- Display distance measurement

Code:
[Ultrasonic Test](Code/Ultrasonic_Test.ino)

---

# Mini Challenge

## Wake Up the Vehicle

Each team must demonstrate:

✅ Correct wiring

✅ Servo steering movement

✅ Motor movement

✅ IR sensor detection

✅ Ultrasonic distance measurement

before proceeding to Module 2.

---

# Reflection Questions

1. What is the role of the ESP32 in an autonomous vehicle?
2. Why is a motor driver required?
3. What is the purpose of the servo motor?
4. How do IR sensors help a vehicle follow a line?
5. How does an ultrasonic sensor detect obstacles?

---

# Summary

In this module, students learned the hardware architecture of an autonomous vehicle, assembled the NxGV vehicle, connected all components, and verified proper hardware operation through practical testing.

---

## Next Module

➡️ [Module 2: Motor Control](../Module02_Motor_Control/)
