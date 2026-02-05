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
```
2️⃣ Create Virtual Environment (Recommended)
Windows
```bash
python -m venv venv
venv\Scripts\activate
```
Linux / macOS
```bash
python3 -m venv venv
source venv/bin/activate
```

3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

⚠️ On first run, YOLOv8 weights (yolov8n.pt) will download automatically.

▶️ Run the Project
```bash
python main.py
```
```bash
Press ESC to stop the application

Logs will be saved in logs.txt

Video recordings will be saved automatically

📊 Sample Log Output
```bash
[2026-02-02 15:40:01] Object appeared: backpack (ID 3)
[2026-02-02 15:40:12] Abandoned object: backpack (ID 3)
[2026-02-02 15:40:30] Object removed: backpack (ID 3)
```
❌ Common Issues & Fixes
Camera not opening

Try changing the camera index in main.py:

cap = cv2.VideoCapture(1)

pip not recognized (Windows)
```bash
python -m pip install -r requirements.txt
```

⚠️ Limitations

Object IDs are temporary (not real-world identity)

Performance depends on lighting and camera quality

Face recognition is not included (future scope)

🔮 Future Enhancements

Face recognition for suspect identification

Object re-identification across cameras

Email / SMS alerts

Web dashboard for logs and recordings

Cloud storage integration

📜 License

This project is licensed under the MIT License.

👨‍💻 Author

Quantumdynamosmvp
AI & Computer Vision Project


---

## ✅ LAST STEP (Push to GitHub)

CMD me run kar:

```bat
git add README.md
git commit -m "Fixed README formatting with proper command blocks"
git push
