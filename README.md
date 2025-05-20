# GlycoFlow 🌬️
A non-invasive prototype device that estimates average blood sugar levels through breath analysis. Built using an ESP32, OLED display, and a gas sensor, this project is designed for low-cost, portable glucose trend detection without the need for blood samples.

![Image](https://github.com/user-attachments/assets/7ac551fa-5907-422c-b7b5-275a3037ed79)

> ⚠️ Note: The current version is a proof of concept and not medically accurate.It is not ment to completly replace a medical grade glucometer!(The actual project is a work in progress and not the final product)

## 🧠 Main Goals of the project.
This project aims to explore a non-invasive, low-cost alternative to traditional blood glucose monitoring. While glucose meters have become more affordable, the cost of test strips remains a recurring burden for many people — especially those who need to check their levels multiple times a day. By using breath analysis to estimate average blood sugar levels, this prototype offers a potential solution that reduces pain, cost, and inconvenience. The long-term goal is to improve accessibility and quality of life for individuals managing Type 1 or Type 2 diabetes through affordable, user-friendly technology.

The goal of this project is to create a flexible, community-driven platform for non-invasive blood sugar monitoring. The device can be purchased either fully assembled or as a DIY kit — both priced equally — making it accessible to everyone, regardless of technical background. Built on open-source hardware and software, it allows anyone with programming or electronics knowledge to upgrade or improve the system over time. Even the 3D-printed case design is open-source, making it possible to print using eco-friendly materials like recycled plastic, promoting sustainability alongside health. This project encourages collaboration between tech-savvy individuals and everyday users to improve the quality of life for people with Type 1 and Type 2 diabetes, growing into a customizable solution that evolves with both technology and user needs.

---

## 🔧 Components
- ESP32
- OLED Display (0.96” I2C)
- Gas Sensor (currently using MQ2/MQ135)
- Rechargable battery
- 3D printed case

---

## 🧪 Concept
When a person blows into the device, the sensor detects gases in the breath. These values are processed by the ESP32, and an **estimated average blood sugar level** is shown on the OLED display. 
---
## ⚙️ How It Works
This device estimates blood glucose levels through breath analysis using a gas sensor. On first use, the user is prompted to calibrate the system:

- ### Calibration Phase (First-Time Setup):

The user blows into the sensor when prompted.
Once the sensor readings stabilize, the device displays them.
The user checks their glucose level with a medical-grade glucometer (e.g., Accu-Chek).
They then input or confirm the actual value, allowing the device to map the breath reading to a real glucose level.

- ### Measurement Phase (After Setup):
On pressing a button, the device enters measurement mode.
The user blows into the device again.
While the sensor value is fluctuating, the screen displays "Measuring...".
Once the value stabilizes, the screen updates to show the estimated blood glucose level.

- ### Learning & Accuracy Improvement:
Over time, the system learns individual trends based on repeated calibration checks.
This helps improve accuracy by adjusting to each person’s unique breath profile.
The design prioritizes ease of use, low cost, and modifiability, making it ideal for open-source development and community-driven improvement.
### TLDR
The device uses breath analysis to estimate blood glucose levels. On first use, the user calibrates it by blowing into the sensor and confirming their actual glucose level using a medical-grade glucometer. The device maps sensor data to this value for accuracy.

During normal use, the user blows into the device after pressing a button. While readings fluctuate, it shows "Measuring...". Once stable, it displays the estimated glucose level. Over time, it learns user trends to improve accuracy.



---
## Prototypes:
![Image](https://github.com/user-attachments/assets/7ac551fa-5907-422c-b7b5-275a3037ed79)

![Image](https://github.com/user-attachments/assets/7ba2b4c4-64ce-486c-9811-8a954e562218)
## Prototype 3D model.

![Image](https://github.com/user-attachments/assets/70ac423a-04b4-4a4e-98d3-cd8d95f93d65)

![Image](https://github.com/user-attachments/assets/63d26681-e3f9-4f48-a3fd-c56b0c87fe26)
---
## 📈 Future Ideas
- Bluetooth logging to mobile app
- Use a machine learning model to improve accuracy
- Upgrade to acetone-specific sensors
---
## Final concept📃
![Image](https://github.com/user-attachments/assets/cd53f498-e3e6-4253-aa40-fd2f7edba45a)
---

## 🏁 Status
🚧 In development – code and hardware design coming soon!
