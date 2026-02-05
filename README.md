# Object & Asset Security Monitoring System

An **AI-based real-time surveillance system** that detects:
- Abandoned objects
- Object removal (theft detection)
- Asset movement history

The project uses **Deep Learning and Computer Vision** to monitor a live camera feed and generate time-stamped security logs with video evidence.

---

## 📌 Key Highlights

- AI-powered object detection using YOLOv8
- Real-time multi-object tracking using DeepSORT
- Logs object appearance, abandonment, and removal
- Each event is logged with:
  - Object type (e.g. backpack, bottle, laptop)
  - Unique tracking ID
  - Timestamp
- Displays live time on camera feed
- Records video automatically for evidence

---

## 🚀 Features

- 📷 Live camera monitoring
- 🧠 AI-based object classification
- 🆔 Temporary object ID assignment
- ⏱ Time-based abandoned object detection
- 🚨 Theft detection via object removal
- 📝 Timestamped log generation
- 🎥 Automatic video recording

---

## 🛠 Tech Stack

- **Python** 3.9 or higher  
- **YOLOv8** (Ultralytics) – Object Detection (AI / Deep Learning)  
- **DeepSORT** – Multi-object tracking  
- **OpenCV** – Video processing  
- **NumPy** – Numerical operations  

---

## 📂 Project Structure

asset-security-monitoring/
│
├── main.py # Main application file
├── requirements.txt # Python dependencies
├── README.md # Project documentation
├── .gitignore
├── logs.txt # Auto-generated logs
├── snapshots/ # Saved images (optional)
└── recordings/ # Recorded videos


---

## ⚙️ System Requirements

- Windows / Linux / macOS
- Python 3.9+
- Webcam or external camera
- Internet (first run only, for YOLO model download)

---

## 🧩 Installation & Setup (Step-by-Step)

### 🔹 1. Clone the Repository
git clone https://github.com/Quantumdynamosmvp/asset-security-monitoring.git
cd asset-security-monitoring
🔹 2. Create Virtual Environment (Recommended)
Windows

python -m venv venv
venv\Scripts\activate
Linux / macOS

python3 -m venv venv
source venv/bin/activate
🔹 3. Install Dependencies
pip install -r requirements.txt
⚠️ On first run, YOLOv8 weights (yolov8n.pt) will download automatically.

▶️ Run the Project
python main.py
Press ESC to stop the application.

Logs will be saved in logs.txt

Video recordings will be saved automatically.

📊 Sample Log Output
[2026-02-02 15:40:01] Object appeared: backpack (ID 3)
[2026-02-02 15:40:12] Abandoned object: backpack (ID 3)
[2026-02-02 15:40:30] Object removed: backpack (ID 3)
🧠 How the System Works
Camera captures live video frames.

YOLOv8 (AI model) detects objects and their types.

DeepSORT assigns temporary IDs and tracks movement.

Logic engine checks:

Object appeared

Object static for long time (abandoned)

Object disappeared (removed)

Events are logged with timestamp and object details.

Video is recorded for evidence.

🎯 Use Cases
Theft detection in shops and warehouses

Monitoring assets in offices, labs, and classrooms

Abandoned bag detection in public places

Inventory safety and security auditing

⚠️ Limitations
Object IDs are temporary (not real-world identity)

Performance depends on lighting and camera quality

Not designed for face or ownership recognition (future scope)

🔮 Future Enhancements
Face recognition for suspect identification

Object re-identification across cameras

Email / SMS alerts

Web dashboard for logs and recordings

Cloud storage integration

🐞 Common Issues & Fixes
❌ Camera not opening
Try changing camera index in main.py:

cap = cv2.VideoCapture(1)
❌ pip not recognized (Windows)
Use:

python -m pip install -r requirements.txt
📜 License
This project is licensed under the MIT License.

👨‍💻 Author
Quantumdynamosmvp
AI & Computer Vision Project


---

# ✅ Next Steps (very quick)

CMD me run:
bat
git add README.md
git commit -m "Improved README with detailed setup and commands"
git push
