# Arduino-Ultrasonic-Servo-Control

## Overview

This project demonstrates how to control a Servo Motor using an HC-SR04 Ultrasonic Sensor with an Arduino Uno.

The ultrasonic sensor continuously measures the distance to nearby objects. When an object is detected within 10 cm, the servo motor rotates to 90°, and an LED turns on. When the object moves farther than 10 cm, the servo returns to its initial position (0°), and the LED turns off.

This project was implemented and tested using real Arduino hardware.

---

## Components

- Arduino Uno
- HC-SR04 Ultrasonic Sensor
- SG90 Servo Motor
- LED
- 220Ω Resistor
- Breadboard
- Jumper Wires
- USB Cable

---

## Circuit Connections

### Servo Motor

| Servo Pin | Arduino |
|-----------|----------|
| Signal | D9 |
| VCC | 5V |
| GND | GND |

### HC-SR04

| Sensor Pin | Arduino |
|------------|----------|
| VCC | 5V |
| TRIG | D10 |
| ECHO | D11 |
| GND | GND |

### LED

| LED | Arduino |
|------|----------|
| Positive | D7 (through 220Ω resistor) |
| Negative | GND |

---

## Program Logic

1. Measure the distance using the HC-SR04 ultrasonic sensor.
2. If the detected distance is **10 cm or less**:
   - Rotate the servo motor to **90°**.
   - Turn on the LED.
3. If the distance is **greater than 10 cm**:
   - Return the servo motor to **0°**.
   - Turn off the LED.

---

## Files

```
Arduino-Ultrasonic-Servo-Control
│
├── Servo_Ultrasonic.ino
├── README.md
└── Images
    ├── circuit_90degree.mov
    ├── circuit_180degree_15cm.mov
    └── working.mov
```

---

## Result

The system successfully detects nearby objects using the HC-SR04 ultrasonic sensor. When an object is detected within 10 cm, the servo rotates to 90° and the LED turns on. When the object moves away, the servo returns to 0° and the LED turns off.

<img width="959" height="772" alt="Fabulous Blad" src="https://github.com/user-attachments/assets/50078ca9-523c-4e1c-80ea-4e8a63b16244" />


---

## Author

Developed by **Aljazi Alghamdi**
