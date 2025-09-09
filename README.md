
# MediTrack: Smart Pill Dispenser for Elderly Care

MediTrack is an **AI-powered smart medication dispenser** designed to help elderly individuals and patients with chronic illnesses adhere to their medication schedules. It integrates **IoT, Artificial Intelligence (AI), and mobile connectivity** to ensure timely, accurate, and personalized medication management.

---

## 🚀 Features

- **Automated Pill Dispensing**: Rotatory blister pack carousel for 7–14 medications.
- **Real-Time Adherence Tracking**: Light sensors verify pill removal; missed doses trigger alerts.
- **AI-Powered Monitoring**:
  - Predicts non-adherence patterns using **LSTM/ARIMA** models.
  - Adaptive rescheduling with **reinforcement learning**.
- **Mobile App (Android)**:
  - Patient view: reminders, confirmation, optional photo verification.
  - Caregiver view: logs, trend reports, alerts, remote overrides.
- **Voice Interaction**: NLP-based voice commands (e.g., “When is my next dose?”).
- **Multi-Channel Alerts**: Local alarms, push notifications, SMS, and caregiver updates.
- **Offline Reliability**: Edge processing on **ESP32** with RTC and power backup.
- **Compact & Hygienic Design**: ~30×25×15 cm, blister pack support for minimal handling.

---

## 🛠️ Technical Specifications

| Category       | Component                     | Description |
|----------------|-------------------------------|-------------|
| **Processor**  | ESP32 Microcontroller         | Core logic, Wi-Fi & BLE |
| **Timekeeping**| DS3231 RTC Module             | Precision scheduling |
| **Mechanical** | Rotatory Carousel + Servo     | Holds blister packs (7–14 slots) |
| **Sensors**    | LDR, Push Buttons             | Adherence tracking & manual overrides |
| **Display**    | OLED (0.96” I2C)              | Medication prompts, menus |
| **Alerts**     | Buzzer + LED Indicators       | Audio-visual reminders |
| **Power**      | 2×18650 Li-ion Battery + RTC backup | Long runtime & resilience |
| **Software**   | Android App + Firebase Realtime DB | Scheduling & caregiver dashboard |
| **AI Models**  | LSTM, ARIMA, Reinforcement Learning | Predictive analytics & adaptive schedules |
| **NLP/Voice**  | TensorFlow Lite + Google Speech API | Voice-enabled interface |

---

## 📱 Mobile Application

- **Patient Interface**
  - Reminders with sound, vibration, and on-screen alerts.
  - "Taken" confirmation button with optional photo upload.
  - Voice command support for accessibility.

- **Caregiver Interface**
  - Real-time adherence dashboard.
  - Weekly/monthly compliance reports.
  - Remote schedule management & emergency overrides.
  - Multi-channel alerts for missed doses.

---

## 🔬 How It Works

1. **Setup**: Caregiver programs medication schedule via app or device interface.
2. **Dispense**: At scheduled time, carousel rotates to correct blister pack slot.
3. **Notify**: Buzzer, LED, and OLED display prompt the patient.
4. **Verify**: LDR sensor checks pill removal. If not taken within ~5 minutes → caregiver notified.
5. **Log & Analyze**: Data stored locally and synced to the app, AI detects trends for predictive adherence support.

---

## 📊 Advantages Over Traditional Pill Dispensers

- AI-driven **predictive monitoring** (not just reactive logging).
- Adaptive, personalized schedules (vs. fixed alarms).
- Direct blister-pack integration (avoids manual pill sorting, improves hygiene).
- Real-time **objective adherence verification** with sensor + optional photo.
- Voice interface for accessibility.
- Redundant notifications (local + mobile + SMS).
- Scalable design for home and clinical use.

---

## 📐 Dimensions

- Device Size: **~30 × 25 × 15 cm**
- Carousel: **7–14 blister pack slots**
- Weight: **~1.2 kg**
- Power Backup: **Rechargeable Li-ion + RTC coin-cell**

---

## 📸 Prototype & App Screens

- Hardware Prototype: Rotatory blister carousel with ESP32 and OLED.
- Mobile App: Caregiver & patient dashboard with adherence tracking.

<img width="964" height="1112" alt="image" src="https://github.com/user-attachments/assets/6e76871b-2570-4050-89a7-84eb16537160" />



<img width="430" height="430" alt="image" src="https://github.com/user-attachments/assets/3694b1a3-fa95-4f4b-805b-4c90e1fe3e68" />

 
 <img width="430" height="430" alt="image" src="https://github.com/user-attachments/assets/9e9a9dcc-71d2-427c-99f4-de46f24a3919" />

 
 <img width="262" height="530" alt="image" src="https://github.com/user-attachments/assets/237669cf-6077-44b9-84b0-5ab5e3d52927" />




---

## 👨‍💻 Contributors

- **Prajes Das**  
- **Sukalyan Chakraborty**  
- **Dr. Shubhendu Banerjee**

---

