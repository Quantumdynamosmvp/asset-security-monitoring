# 🛡️ Object & Asset Security Monitoring System

An AI-powered real-time surveillance project that detects:
- 📍 Object appearance
- 🧍 Abandoned objects
- 🚨 Object removal (theft detection)
- 📋 Generates timestamped logs
- 🎥 Records video evidence

This system uses YOLOv8 and DeepSORT for tracking and provides easy-to-run steps for beginners.

---

## 📌 Features

✔ **Real-time object monitoring**  
✔ **Object classification** (e.g., backpack, laptop)  
✔ **Multi-object tracking with temporary IDs**  
✔ **Abandoned object detection**  
✔ **Object removal / theft detection**  
✔ **Live timestamp overlay on video**  
✔ **Event logs with timestamps**
✔ **Video recording for evidence**

---

## 🧠 How It Works

1. **YOLOv8** (Deep Learning model) detects objects frame by frame.
2. **DeepSORT** tracker assigns consistent IDs to detected objects.
3. The logic module checks:
   - If an object appears → logs appear event
   - If an object stays in place for too long → logs abandoned event
   - If an object disappears → logs removed event
4. **Logs** are stored with object name, ID & time.
5. **Live feed** shows detections and time overlay.
6. **Recorded video** stored automatically.

---

## 📂 Repo File Structure

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

✔ Python 3.9 or higher  
✔ Webcam / Camera  
✔ Command Line (Terminal / PowerShell)  
✔ Internet connection (first run for model weights)

---

## 🚀 Installation (Step-by-Step)

### 1️⃣ Clone the GitHub repository
```bash
git clone https://github.com/Quantumdynamosmvp/asset-security-monitoring.git
cd asset-security-monitoring
2️⃣ Create Virtual Environment (Recommended)
Windows:

python -m venv venv
venv\Scripts\activate
Linux / macOS:

python3 -m venv venv
source venv/bin/activate
3️⃣ Install Dependencies
pip install -r requirements.txt
⚠️ On first run, YOLOv8 will automatically download its weights (yolov8n.pt).

▶️ Run the Project
python main.py
Press ESC to stop the program.

Live video will show detections with live timestamps.

All events will be logged in logs.txt.

Video will be recorded in the recordings/ folder.

📊 Example Log Output
[2026-02-02 15:40:01] Object appeared: backpack (ID 3)
[2026-02-02 15:40:12] Abandoned object: backpack (ID 3)
[2026-02-02 15:40:30] Object removed: backpack (ID 3)
🖼 Visual Output Examples
📌 (Add these screenshots to your repo under an assets/ folder.)

👁️ Live Detection with Time Overlay
assets/live_detection.png

📄 Logs Output
assets/logs.png

🎞 Recorded Video Frame
assets/recording.png

⚠️ Common Issues & Fixes
❌ Camera Not Opening
Try changing camera index:

cap = cv2.VideoCapture(1)
❌ pip Not Recognized (Windows)
python -m pip install -r requirements.txt
💡 Tips
✔ Run in a well-lit area for better detection
✔ If too many objects, reduce detection classes in code
✔ Ignore zones configurable in main.py

⚙️ Future Enhancements
✔ Email/SMS alerts
✔ Web dashboard
✔ Object re-identification
✔ Multi-camera support
✔ Cloud storage integration

📜 License
Distributed under the MIT License
See LICENSE file for details.

👨‍💻 Author
Quantumdynamosmvp
AI & Computer Vision Enthusiast


---

## ✅ Quick Upload Instructions

After updating README, run:

```bash
git add README.md
git commit -m "Improved professional README"
git push
