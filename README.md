# Object & Asset Security Monitoring System

An AI-based real-time surveillance system for detecting:
- Abandoned objects
- Object removal (theft detection)
- Asset movement history

The system uses:
- YOLOv8 for object detection (Deep Learning)
- DeepSORT for object tracking (unique IDs)
- Timestamp-based event logging
- Video recording and snapshot evidence

---

## 🚀 Features

- Detects objects in real time
- Logs when an object appears in the scene
- Detects abandoned objects (static for defined time)
- Detects object removal (disappearance from scene)
- Records:
  - Object type (e.g. backpack, bottle, laptop)
  - Object ID
  - Timestamp
- Displays live time on camera feed
- Saves recorded video for evidence

---

## 🛠 Tech Stack

- Python 3.9+
- OpenCV
- YOLOv8 (Ultralytics)
- DeepSORT (deep-sort-realtime)
- NumPy

---

## 📂 Project Structure

