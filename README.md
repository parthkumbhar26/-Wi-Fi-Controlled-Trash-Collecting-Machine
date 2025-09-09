**WiFi Controlled Trash Collecting Machine**

A **Wi-Fi controlled robot** that moves using a web page hosted on **NodeMCU (ESP8266)**.  
It uses an **L298N motor driver** to drive 4 DC motors (two on each side).  
This version covers **vehicle movement** (Forward/Backward/Left/Right/Stop). You can add the conveyor later.

---

## Features
- Control from any phone/laptop on the same Wi-Fi (no app needed)
- Simple web buttons: **Forward / Backward / Left / Right / Stop**
- Clean, beginner-friendly Arduino sketch
- Conveyor belt control
  
---

## Components
- **NodeMCU (ESP8266)**
- **L298N** motor driver
- 4 × DC motors with wheels
- 1 × DC motor (conveyor belt)
- Conveyor Belt with DC Motor
- Battery pack (match motor voltage)
- Chassis, jumper wires

---

## Wiring (recommended pins)
| Function | NodeMCU Pin | ESP8266 GPIO | L298N |
|---|---:|---:|---|
| Left motor IN1 | D1 | 5  | IN1 (L298N #1) |
| Left motor IN2 | D2 | 4  | IN2 (L298N #1) |
| Right motor IN1 | D5 | 14 | IN3 (L298N #1) |
| Right motor IN2 | D6 | 12 | IN4 (L298N #1) |
| ENA / ENB | — | — | Keep jumpers ON |
| GND | GND | — | Common GND across NodeMCU + L298N + Battery |

---

## ▶️ Controls
- **Forward** → Moves the vehicle ahead.
- **Backward** → Moves the vehicle back.
- **Left** → Turns left.
- **Right** → Turns right.

---

## ⚡ How It Works
1. Connect Arduino to ESP8266 WiFi module.
2. Upload the code from `/code/trash_collector.ino`.
3. Power the circuit with battery supply.
4. Connect your phone/laptop to the same WiFi network.
5. Open the IP shown in Serial Monitor → Control the robot.
