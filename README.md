# 🛡️ Object & Asset Security Monitoring System

An **AI-powered real-time surveillance system** that monitors objects and assets using computer vision.

The system can:
- Detect when an object appears
- Detect abandoned objects
- Detect object removal (theft detection)
- Log events with object name, ID, and timestamp
- Record video evidence automatically

---

## ✨ Features

- 📷 Live camera monitoring  
- 🧠 AI-based object detection (YOLOv8)  
- 🆔 Multi-object tracking with DeepSORT  
- ⏱ Timestamped event logging  
- 🚨 Theft detection via object removal  
- 🎥 Automatic video recording  
- 📝 Human-readable logs  

---

## 🧠 How the System Works

1. Camera captures live video frames.
2. **YOLOv8 (AI model)** detects objects and their categories.
3. **DeepSORT** assigns temporary IDs and tracks object movement.
4. Logic engine checks:
   - Object appeared
   - Object abandoned (static for a defined time)
   - Object removed from the scene
5. Events are logged with **object name, ID, and timestamp**.
6. Video is recorded for security evidence.

---

## 📂 Project Structure

asset-security-monitoring/
│
├── main.py
├── requirements.txt
├── README.md
├── .gitignore
├── logs.txt
├── snapshots/
└── recordings/

---

## 🛠 Prerequisites

- Python **3.9 or higher**
- Webcam / external camera
- Git (optional, for cloning)
- Internet connection (first run only)

---

## 🛠 Prerequisites

- Python **3.9 or higher**
- Webcam / external camera
- Git (optional, for cloning)
- Internet connection (first run only)
---

## ⚙️ Installation & Setup (Step-by-Step)

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Quantumdynamosmvp/asset-security-monitoring.git
cd asset-security-monitoring
