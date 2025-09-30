# 🚗 Arduino Bluetooth RC Car

This project is a **Bluetooth-controlled RC Car** built with Arduino and simple electronic components.  
It demonstrates motor control, PWM-based speed adjustment, and wireless communication using an HC-05 module.  

As a **CSE undergrad passionate about Robotics**, I built this project to sharpen my embedded systems and robotics skills.  

---

## 🔧 Components Used
- Arduino Nano  
- Dual Motor Driver TB6612FNG (1A)  
- N20 Motors (x2)  
- LM2596 DC-DC Buck Converter  
- HC-05 Bluetooth Module  
- Li-ion Battery  

---

## ⚙️ Features
- **Directional Movement**: Forward, Backward, Left, Right  
- **Diagonal Moves**: Forward-Left, Forward-Right, Backward-Left, Backward-Right  

---

## 🎮 Bluetooth Commands
| Command | Action |
|---------|--------|
| `F` | Forward |
| `B` | Backward |
| `L` | Left |
| `R` | Right |
| `G` | Forward-Left |
| `I` | Forward-Right |
| `H` | Backward-Left |
| `J` | Backward-Right |
| `0-9` | Speed Control |
| `S` | Stop |

---

## 📝 Circuit Wiring
| Arduino Pin | Component Connection |
|-------------|----------------------|
| 4 | AIN1 (Motor Driver) |
| 5 | AIN2 (Motor Driver) |
| 3 | PWMA (Motor A PWM) |
| 8 | BIN1 (Motor Driver) |
| 7 | BIN2 (Motor Driver) |
| 6 | PWMB (Motor B PWM) |
| 9 | HC-05 RX (via SoftwareSerial) |
| 10 | HC-05 TX (via SoftwareSerial) |

*(Power managed through LM2596 with Li-ion battery.)*  

---
## 📷 Picture
![WhatsApp Image 2025-09-30 at 08 54 42_aa9ea578](https://github.com/user-attachments/assets/5db3d832-732e-4360-915a-d0c919fdf954)
![WhatsApp Image 2025-09-30 at 08 54 44_3d065a8d](https://github.com/user-attachments/assets/157fb837-2e9e-45cc-9316-4f8a03b47bc8)

## 📷 Demo
<img width="2658" height="1461" alt="RC Car_bb" src="https://github.com/user-attachments/assets/57acddd9-48b6-44a1-98a5-64d76f74be8f" />


---

## 🚀 Future Improvements
- Add ultrasonic sensor for **obstacle avoidance**  
- Add IR sensors for **line following**  
- Add voice control / mobile app integration  
- Add camera module for **FPV (First Person View)**  

---

## 📖 What I Learned
- Motor driver control with PWM  
- Bluetooth communication with HC-05  
- Power management for motors and Arduino  
- Writing modular Arduino code  

---

## 💡 About Me
I’m **Marup Hossain**, a 3rd-year **Computer Science and Engineering (CSE)** undergrad at **American International University-Bangladesh (AIUB)** 🇧🇩.  

👉 Connect with me on [LinkedIn](https://www.linkedin.com/in/marup-hossain-64722834a?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app))  
👉 Explore my other projects on [GitHub](your-github-url](https://sites.google.com/view/maruphossain/home))  

---
