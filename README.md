# 🖱️ Gesture and Voice Controlled Virtual Mouse

This project is a **contactless virtual mouse** that allows users to control their computer using **hand gestures** and **voice commands**, enhancing human-computer interaction (HCI) through real-time computer vision and speech recognition.

---

## 📌 Abstract

The Virtual Mouse system uses a webcam and microphone to detect **hand gestures** and recognize **voice commands** for controlling mouse functions. It’s particularly useful for:

- **Hands-free control** in AR/VR, robotics, classrooms.
- **Assisting specially abled** users.
- **Touchless computing** during health-sensitive situations (like COVID-19).

---

## 🎯 Objectives

- Track hand movement using a webcam to simulate mouse movement and clicks.
- Implement fingertip and knuckle tracking using MediaPipe for gesture control.
- Develop a voice assistant (`Jerry`) using `SpeechRecognition` to:
  - Open folders/files
  - Control mouse actions
  - Perform basic navigation
- Integrate gesture and voice modules into a unified system.

---

## 🧠 Features

### 🎮 Gesture Control

- Move Cursor
- Left/Right Click
- Double Click
- Scroll
- Drag & Drop
- Multi-item Selection
- Volume/Brightness Control

### 🎤 Voice Control

- Launch/Stop Gesture Control
- Google Search
- Find location on Google Maps
- File navigation (open/copy/paste)
- Current date and time
- Sleep/Wakeup app
- Exit app

---

## 🛠️ Methodology

### ✅ Gesture Module
- Uses **OpenCV** for video capture and **MediaPipe** for hand tracking.
- Gesture interpretation based on **21 hand landmarks**.
- Clicks and actions triggered by calculating angles and distances between fingertips.

### ✅ Voice Module
- Voice assistant **"Jerry"** built using `SpeechRecognition`.
- Listens to and interprets user commands in real-time.

---

## 🖼️ Screenshots

> Include output images in a folder `screenshots/` and reference them like this:

### Gesture Control Demo
![Gesture Control](screenshots/gesture_control.png)

### Voice Control Demo
![Voice Assistant](screenshots/voice_assistant.png)

---

## ⚙️ Requirements

### Hardware
- Webcam (≥ 1.3 MP)
- Microphone

### Software
- Python ≥ 3.8
- Libraries:
  - `opencv-python`
  - `mediapipe`
  - `pyautogui`
  - `speechrecognition`
  - `pynput`

Install requirements using:
```bash
pip install -r requirements.txt
