# README — Smart Facial-Recognition Attendance

> Copy into your GitHub repo `facial-recognition-attendance`.

# 🧑‍💼 Smart Facial-Recognition Attendance System

A smart presence/attendance system that identifies people in real time with computer vision and automatically logs attendance — no manual sign-in.

## Features
- 👁️ Real-time face detection and identification (Python + OpenCV)
- ✅ Automatic attendance logging to CSV/Excel with timestamp
- 📊 Simple dashboard of attendance history
- 🔒 Local processing — no cloud dependency (privacy-friendly)

## Stack
`Python` `OpenCV` `face_recognition / Haar cascades` `NumPy` `CSV/Excel export`

## How it works
1. Enrollment: capture reference faces per person
2. Detection loop: detect faces per frame, encode, compare against database
3. On match: log name + timestamp (deduplicated per day)
4. Export: attendance report (CSV) for HR use

## Results
- Real-time recognition on standard webcam (30 fps detection loop)
- Usable in classroom/office attendance scenarios

## Skills demonstrated
`Python` `OpenCV` `Computer vision` `Automation` `Data logging`

## Author
Hassan AIT ALLOU — [LinkedIn](https://www.linkedin.com/in/hassan-ait-allou)
