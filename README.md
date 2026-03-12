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

## Requirement

Android 6.0.0+ (phone)

## ⚙️ How to Setup (Fully Automated Mode)

Forget typing commands every time! SanStats is designed to be a "Plug & Play" experience.

### 1. PC Setup (One-Time Configuration)
1. Install **Python 3** and required libraries via Command Prompt:
   ```bash
   pip install psutil GPUtil
2. Download all files frrom the release sections

Make sure you have ADB installed on your PC, 

important_____
(update the exact ADB path inside the Auto_ADB.bat file.)

3. now make a folder (default folder name in .bat file is- "New folder") 

now, paste the .bat file and .py file in this folder 

4. Automate the Startup:

* Press Win + R, type shell:startup, and hit Enter.
* Paste the SanStats_Server.vbs file into this Startup folder. (This ensures the Python server and ADB listener run silently in the background every time you turn on your PC).

### 2. Android Setup
Download the latest APK from the Releases tab.

Install SanStats.apk on your device from the release section.

Enable USB Debugging in your phone's Developer Options.

### 3. The Magic (Plug & Play) 🪄
Turn on your PC (The background scripts will start automatically).

Connect your Android phone via USB cable.

Open the SanStats app. The scripts will automatically detect your phone, forward the ports, and your meters will instantly go live after the ignition sweep!

## info!!/Not Working?
If not working try to change the path in .bat file and .vbs file from deafult to your own 

Note- this thing is little tough to use for beginners, so do it with lots of patience plzz 

it's 100% working 

## 👨‍💻 Developer

Made with ❤️ by Rishi Sann
