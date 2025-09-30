# Arduino Bluetooth RC Car 🚗

This project is an Arduino-powered RC car controlled via Bluetooth using an HC-05 module.  
It uses TB6612FNG motor driver, N20 motors, and an LM2596 step-down converter powered by Li-ion battery.

---

## 🔧 Components
- Arduino Nano
- TB6612FNG Dual Motor Driver
- N20 Motors
- LM2596 DC-DC Buck Converter
- HC-05 Bluetooth Module
- Li-ion Battery

---

## ⚙️ Features
- Forward, backward, left, right movements
- Diagonal (forward-left, forward-right, backward-left, backward-right)
- Bluetooth control from Android app

---

## 📜 Code
The Arduino code reads Bluetooth commands and controls motor driver pins to move the car.  
Commands supported:  
- `F` → Forward  
- `B` → Backward  
- `L` → Left  
- `R` → Right  
- `G/I/H/J` → Diagonal moves  
- `0-9` → Speed control  
- `S` → Stop  

---

## 📷 Project Demo
(Add 1–2 pictures of your car setup here. If possible, upload a short GIF or link a YouTube demo.)

---

## 🚀 Future Improvements
- Add obstacle avoidance (ultrasonic sensor)
- Add line following mode
- Add voice control
