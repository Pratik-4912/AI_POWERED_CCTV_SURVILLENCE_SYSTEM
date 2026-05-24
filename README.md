# SafeSight – AI-Powered CCTV Surveillance System

SafeSight is a real-time AI-powered surveillance system built using computer vision and deep learning to monitor CCTV feeds and detect security-critical events automatically.

It can detect events such as:

- Intrusion Detection
- Crowd Formation Detection
- Fire Detection
- Human Fall Detection
- Loitering Detection
- Person Detection & Tracking
- Face Recognition (optional)

When an event is detected, SafeSight can generate alerts, capture snapshots, log incidents, and send Telegram notifications instantly.

---

## Features

### Person Detection & Tracking
Uses YOLO to detect and track people in real time from CCTV footage.

### Intrusion Detection
Detects when a person enters a restricted Region of Interest (ROI).

### Loitering Detection
Tracks dwell time and flags suspicious long-duration presence.

### Crowd Detection
Detects crowd formation using density/grid-based analysis.

### Fire Detection
Identifies possible fire regions using computer vision-based color segmentation.

### Fall Detection
Uses MediaPipe Pose estimation to detect human falls.

### Face Recognition (Optional)
Supports face recognition using LBPH.

### Event Logging
Stores event logs with timestamp and exports to CSV.

### Snapshot Capture
Captures event images automatically.

### Telegram Alerts
Sends instant alert notifications with images to Telegram.

### Live Dashboard Metrics
Displays:
- FPS
- Detection latency
- Alert count
- Event monitoring status

---

# Tech Stack

- Python
- OpenCV
- NumPy
- Flask
- YOLO (Ultralytics)
- MediaPipe

---

# Project Structure

```bash
SafeSight/
│
├── dashboard/
│   ├── app.py
│   ├── templates/
│   └── static/
│
├── detection/
│   └── yolo_detector.py
│
├── data/
│   ├── videos/
│   └── faces/
│
├── main.py
├── requirements.txt
└── README.md
```

---

# Installation

## Clone Repository

```bash
git clone https://github.com/Pratik-4912/AI_POWERED_CCTV_SURVILLENCE_SYSTEM.git
cd AI_POWERED_CCTV_SURVILLENCE_SYSTEM
```

---

## Create Virtual Environment

```bash
python -m venv venv
```

Activate:

### Windows

```bash
venv\Scripts\activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Run Project

## Main Detection System

```bash
python main.py
```

## Run Dashboard

```bash
cd dashboard
python app.py
```

---

# Open in Browser

```bash
http://127.0.0.1:5000/
```
# API Endpoints

| Endpoint | Description |
|---|---:|
| `/video_feed` | Live CCTV stream |
| `/toggle_crowd` | Enable/Disable crowd detection |
| `/toggle_fire` | Enable/Disable fire detection |
| `/toggle_fall` | Enable/Disable fall detection |
| `/toggle_face` | Enable/Disable face recognition |
| `/events` | View event logs |
| `/metrics` | Live system metrics |

---
# Telegram Alert Setup

Add your Telegram bot credentials inside the code:

```python
BOT_TOKEN = "YOUR_BOT_TOKEN"
CHAT_ID = "YOUR_CHAT_ID"
```
# Author

## Pratik

GitHub:

https://github.com/Pratik-4912

Project Repository:

https://github.com/Pratik-4912/AI_POWERED_CCTV_SURVILLENCE_SYSTEM

---
# Future Improvements

- Multi-camera support
- Email alerts
- Cloud deployment
- Database-based event storage
- Mobile alert dashboard
- Advanced face recognition with embeddings

# License

This project is built for academic and learning purposes.
