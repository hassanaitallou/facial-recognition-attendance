# Smart Facial-Recognition Attendance System

A presence/attendance system that identifies people in real time with computer vision and automatically logs attendance — no manual sign-in required.

## Overview

The system captures video from a camera, detects faces, compares them against an enrolled database and records attendance with a timestamp. Processing is local — no cloud dependency.

## Objectives

- Real-time face detection and identification
- Automatic, timestamped attendance logging
- Simple enrollment and reporting
- Privacy-friendly local processing

## Features

- Real-time face detection and recognition (Python + OpenCV)
- Automatic attendance logging to CSV / Excel
- Attendance history dashboard
- Deduplication per day
- Local processing — no cloud dependency

## Architecture

```
Camera frame → Face detection (Haar / DNN) → Face encoding
        → Comparison against enrolled database
        → On match: log name + timestamp (deduplicated per day)
        → Export attendance report
```

## Software

`Python` · `OpenCV` · `face recognition / Haar cascades` · `NumPy` · `CSV / Excel export`

## Installation

```bash
pip install opencv-python numpy
```

## Usage

1. **Enrollment** — capture reference faces for each person.
2. **Detection loop** — detect faces per frame, encode and compare against the database.
3. **On match** — log name + timestamp (deduplicated per day).
4. **Export** — generate the attendance report (CSV / Excel).

## Results

- Real-time detection and identification validated
- Automatic, timestamped attendance records
- Designed for classrooms and controlled-access areas

## Future Improvements

- Edge deployment on a small PC / Jetson
- Anti-spoofing (liveness detection)
- Integration with an MQTT dashboard
