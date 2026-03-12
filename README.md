# 🚀 SanStats - Custom PC Hardware Monitor

Turn your old, unused Android phone into a premium, real-time PC hardware monitor! **SanStats** is a custom-built solution that displays your PC's live performance stats directly on an Android device via a zero-latency USB connection.

Developed using **Python** (Server-side) and **Java/Android** (Client-side).

## ✨ Features
* **Zero Latency Connection:** Uses USB and ADB Reverse Port Forwarding. No Wi-Fi or Bluetooth required!
* **Real-Time Data:** Live monitoring of CPU usage, GPU load (Nvidia), RAM usage, GPU Temperature, and Storage (C: & D: Drives).
* **Premium Custom UI:** Features a sleek, dark-mode dashboard with custom-built horseshoe gauge meters and unique color coding.
* **Ignition Animation:** A smooth, sports-car-style sweep animation on the dashboard every time the app starts.
* **Highly Optimized:** Designed to run flawlessly even on older devices (Tested on Android 6.0 Marshmallow).
* **Fully Automated (Plug & Play):** Includes background scripts that automatically start the PC server and bridge the connection the moment you plug in your phone.

## 🛠️ Tech Stack
* **PC Server:** Python 3, `socket`, `psutil`, `GPUtil`
* **Android Client:** Java, Custom Canvas Views (for Gauges), Android SDK
* **Automation:** Windows VBScript & Batch Scripting, ADB (Android Debug Bridge)

## 📸 Preview
*(Note: Replace preview.jpg with your uploaded image name)*
![SanStats UI](preview.jpg)

## ⚙️ How to Setup (Fully Automated Mode)

Forget typing commands every time! SanStats is designed to be a "Plug & Play" experience.

### 1. PC Setup (One-Time Configuration)
1. Install **Python 3** and required libraries via Command Prompt:
   ```bash
   pip install psutil GPUtil
