# 🚨 Ultrasonic Obstacle Detection System

A simple obstacle detection and warning system built using:

- ESP32 / Arduino
- HC-SR04 Ultrasonic Sensor
- Buzzer

The system continuously measures distance and activates a buzzer whenever an object comes within a defined threshold range.

---

# 🚀 Features

✅ Real-time distance measurement  
✅ Obstacle detection using ultrasonic sensor  
✅ Automatic buzzer alert  
✅ Adjustable detection threshold  
✅ Simple and lightweight code  
✅ Beginner-friendly electronics project  

---

# 🛠 Hardware Used

| Component | Quantity |
|---|---|
| ESP32 / Arduino | 1 |
| HC-SR04 Ultrasonic Sensor | 1 |
| Active Buzzer | 1 |
| Jumper Wires | Few |

---

# 🔌 Wiring

## HC-SR04 → ESP32

| HC-SR04 Pin | ESP32 Pin |
|---|---|
| VCC | 5V |
| GND | GND |
| TRIG | GPIO 4 |
| ECHO | GPIO 5 |

## Buzzer → ESP32

| Buzzer Pin | ESP32 Pin |
|---|---|
| Positive (+) | GPIO 6 |
| Negative (-) | GND |

---

# ⚙ Working Principle

1. Ultrasonic sensor sends sound pulse
2. Echo pin receives reflected pulse
3. Distance is calculated
4. If object distance is below threshold:
   - Buzzer turns ON
5. If no object detected:
   - Buzzer stays OFF

---

# 📏 Detection Threshold

Current threshold:

```cpp
#define THRESHOLD_CM 30
```

If object is closer than:

```text
30 cm
```

the buzzer activates.

---

# 🖥 Serial Monitor Output

Example:

```text
Distance: 25 cm
Distance: 18 cm
Distance: 10 cm
```

If object is out of range:

```text
No object detected (out of range)
```

---

# 📚 How Distance is Calculated

The ultrasonic sensor measures echo travel time.

Distance formula:

0

Where:

- `d` = distance
- `v` = speed of sound
- `t` = echo time

---

# 🔥 Applications

- Blind assistance systems
- Obstacle avoidance robots
- Parking sensors
- Smart alarms
- Distance measurement systems

---

# 🚀 Future Improvements

- Add OLED display
- Add vibration motor
- Add Bluetooth alerts
- Add battery system
- Add multiple sensors
- Add voice warnings

---

# 👨‍💻 Author

**Hussain Shaikh**

GitHub: `@shkhussain17`

---

# 📄 License

This project is open-source and free to use.