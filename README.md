# 🌀 WindMaster 5000

**A Python-GUI controlled smart fan system with Arduino, real-time current monitoring, preset profiles, and data logging.**

---

## 🚀 Features

* Control fan speed via GUI slider (0–255 PWM)
* Preset fan modes: Low / Medium / Fast / Turbo
* ON/OFF toggle button
* Live current monitoring using ACS712
* Status display with FAULT and OK messages


---

## 🛠️ Hardware Used

* Arduino Uno
* 12V DC Fan
* ACS712 Current Sensor (5A/20A/30A variant)
* N-Channel MOSFET (e.g., IRF540N or IRLZ44N)
* 220Ω gate resistor
* 10kΩ pull-down resistor (gate to GND)
* Flyback diode (e.g., 1N5819 or 1N4007)
* Breadboard + jumper wires
* External 12V power supply

---

## 🔌 How It Works

1. The Python GUI sends fan speed (0–255) over serial to the Arduino.
2. Arduino sets PWM output to fan via MOSFET.
3. ACS712 sensor measures real-time current.
4. Arduino sends back current value as `CURR:0.42`.
5. GUI displays live current and logs data with timestamp.

---

## 📸 GUI Preview
<img width="593" height="265" alt="image" src="https://github.com/user-attachments/assets/44d5f045-59cb-45ab-879c-be2a3a7f6f18" />




---

## 🧠 Built With

* Python 3
* Tkinter
* PySerial
* Arduino IDE

