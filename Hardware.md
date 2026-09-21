<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6982cd7d-0ba7-4cb1-b338-6fa7d47f6a9a" />## 🔬 Hardware Setup

The experimental setup consists of an ECG sensor module connected to an Arduino UNO. The Arduino is connected to the computer through USB for programming and serial data transmission.
<img width="720" height="1280" alt="WhatsApp Image 2026-09-21 at 23 38 40" src="https://github.com/user-attachments/assets/8d66dae0-e95e-4528-9a0e-6bfe05b5f0d1" />
<p align="center">
  <img src="images/ecg-arduino-setup.jpg" width="650">
</p>

<p align="center">
  <b>Figure 1: ECG sensor and Arduino UNO based data acquisition setup</b>
</p>
## SYSTEM ARCHITECHURE

        👤 HUMAN SUBJECT
              │
              ▼
      🫀 ECG ELECTRODES
              │
              ▼
       🩺 ECG SENSOR
              │
              │ Analog ECG Signal
              ▼
        🔵 ARDUINO UNO
              │
              │ ADC
              ▼
      📊 DIGITAL ECG DATA
              │
              ▼
       💻 SERIAL / COM PORT
              │
              ▼
       📈 ECG WAVEFORM
              │
              ▼
      🔬 SIGNAL PROCESSING
              │
              ▼
       🧠 FEATURE EXTRACTION
              │
              ▼
       🎯 CONTROL LOGIC
              │
              ▼
       🚗 ROBOTIC VEHICLE
       
```

