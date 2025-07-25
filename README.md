# 👶 Smart Cradle for Baby Monitoring

An embedded system-based smart cradle that automatically detects baby discomfort through sound and wetness sensors and responds by gently rocking the cradle using servo motors. Built using Arduino and designed to enhance infant care through automation.

---

## 🧩 Problem Statement

Caring for infants requires constant attention to factors like crying and diaper wetness, which can cause discomfort and stress for both the baby and caregivers. This project addresses the need for a responsive system that can detect when a baby is crying or if the diaper is wet and act accordingly by alerting and soothing the baby through rocking.

---

## 🔍 Sensors and Actuators

- **Sound Sensor**: Detects crying or loud noise.
- **Moisture Sensor**: Detects wet diaper condition.
- **Servo Motors (2)**: Controls cradle rocking motion.
- **LED Indicator**: Alerts when diaper is wet.

---

## 🧠 System Logic

- If **moisture** level is above a threshold → LED turns on → `Diaper is wet` message in Serial Monitor.
- If **sound** is detected → `Baby is crying` message appears → cradle rocks automatically using two servo motors.
- Rocking involves oscillating motion through servo sweeps.

---

## 🧪 How It Works

### 🧾 Setup
- Moisture sensor connected to analog pin A0
- Sound sensor connected to digital pin 2
- Servo 1 on pin 5
- Servo 2 on pin 6
- LED indicator on pin 7

### 💡 Sample Code Logic
```cpp
if (moistureValue > threshold)
    -> Turn on LED
if (soundDetected == HIGH)
    -> Trigger servo rocking motion
```

---

## ⚙️ Components Required

| Component        | Quantity |
|------------------|----------|
| Arduino UNO      | 1        |
| Sound Sensor     | 1        |
| Moisture Sensor  | 1        |
| Servo Motor (SG90 or similar) | 2  |
| LED              | 1        |
| Resistors, Wires | As needed |

---

## 🚀 How to Run

1️⃣ Upload the Arduino sketch to your board using Arduino IDE  
2️⃣ Power the board using USB or external supply  
3️⃣ Monitor outputs via Serial Monitor (9600 baud)

---

## 📦 Dependencies

- Arduino IDE
- Servo.h library

---

## 🛠️ Technologies Used

- Embedded C
- Arduino IDE
- Servo control
- Analog/Digital sensor integration

---

⭐ **Star this repo if you found it useful for your baby monitoring or embedded system project!**
