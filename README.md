# Tyran-DualMode-Robot
Tyran — Dual-Mode Autonomous Robot

A versatile Arduino-based mobile robot capable of autonomous navigation (line following + destination searching) and manual Bluetooth control with a servo gripper.
Designed for flexibility, expandability, and educational robotics projects.

🚀 Features
🔹 Autonomous Mode

PID line following using IR sensors

Destination detection logic

Obstacle awareness using ultrasonic sensor (if included)

🔹 Manual Mode

Bluetooth HC-05 remote control

Servo-controlled gripper (2× SG90) for picking and placing

Smooth proportional motor speed control

🔹 Display System

OLED screen for:

Mode indication

Sensor readings

Debug info

🧠 System Overview

Tyran operates in two switches modes:

Mode	Description
Autonomous	Follows line path, searches for specific patterns/destinations, executes defined tasks.
Manual	Controlled via Bluetooth app; joystick-like movement + gripper control.
🔧 Hardware Used
Component	Description
Arduino UNO	Main microcontroller
L298N Motor Driver	Drives dual DC motors
OLED 128×64	Display system
HC-05	Bluetooth module
SG90 Servo × 2	Gripper mechanism
18650 Battery ×5	Power supply
2-Wheel Motor Chassis	Base platform
IR Sensors	Line tracking
Ultrasonic Sensor (Optional)	Obstacle detection
🪛 Pin Connections

(Adjust according to your code — here is a template)

Motor Driver (L298N)
Function	Arduino Pin
ENA	3
IN1	12
IN2	11
IN3	7
IN4	6
ENB	5
Bluetooth HC-05
HC-05 Pin	Arduino Pin
TX	10 / SoftwareSerial RX
RX	9 / SoftwareSerial TX
Ultrasonic Sensor
Function	Pin
Trig	A5
Echo	2
Servos
Servo	Pin
Gripper Servo 1	8
Gripper Servo 2	4
OLED

(Most common: I2C)

Function	Pin
SDA	A4
SCL	A5
