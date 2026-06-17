# 🚗 Driver Monitoring System (ADAS-Like)

## 📌 Overview

The Driver Monitoring System is a Computer Vision-based safety application that monitors a driver's behavior in real time using a webcam. The system detects signs of driver fatigue, drowsiness, microsleep, yawning, gaze distraction, head-down posture, and potential phone usage while driving.

Built using **Python, OpenCV, MediaPipe Face Landmarker, and NumPy**, this project aims to improve road safety by providing real-time alerts when unsafe driving behavior is detected.

---

## 🎯 Features

### 👁️ Eye Monitoring

* Eye Aspect Ratio (EAR) calculation
* Blink detection using MediaPipe Blendshapes
* Eye closure duration tracking
* Drowsiness detection
* Microsleep detection

### 😴 Fatigue Detection

* Yawning detection using Mouth Aspect Ratio (MAR)
* Continuous eye closure monitoring
* PERCLOS (Percentage of Eye Closure) calculation

### 👀 Attention Monitoring

* Gaze direction estimation
* Looking Left detection
* Looking Right detection
* Forward gaze detection

### 📱 Distraction Detection

* Head-down posture detection
* Phone distraction detection
* Driver attention monitoring

### 🚨 Alert System

* Audio alarm for drowsiness
* Microsleep warning alerts
* Real-time visual warnings

---

## 🛠️ Technologies Used

| Technology                | Purpose                   |
| ------------------------- | ------------------------- |
| Python                    | Core Programming          |
| OpenCV                    | Video Processing          |
| MediaPipe Face Landmarker | Facial Landmark Detection |
| NumPy                     | Mathematical Computations |
| Winsound                  | Alarm Generation          |

---

## 📂 Project Structure

```text
Driver-Monitoring-System/
│
├── main.py
├── models/
│   └── face_landmarker.task
│
├── README.md
└── requirements.txt
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/Driver-Monitoring-System.git

cd Driver-Monitoring-System
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

Activate Environment

#### Windows

```bash
venv\Scripts\activate
```

#### Linux/Mac

```bash
source venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 📦 Requirements

Create a `requirements.txt` file with:

```txt
opencv-python
mediapipe
numpy
```

---

## ▶️ Run the Project

Update the model path inside the code:

```python
MODEL_PATH = "models/face_landmarker.task"
```

Run:

```bash
python main.py
```

Press **ESC** to exit.

---

## 📊 Detection Metrics

### Eye Aspect Ratio (EAR)

Used for:

* Blink Detection
* Eye Closure Detection
* Drowsiness Analysis

### Mouth Aspect Ratio (MAR)

Used for:

* Yawning Detection

### PERCLOS

Percentage of time the driver's eyes remain closed.

Used as a standard indicator of fatigue.

---

## 🚨 Driver States

| State      | Description                    |
| ---------- | ------------------------------ |
| NORMAL     | Driver is attentive            |
| DROWSY     | Eyes closed beyond threshold   |
| MICROSLEEP | Prolonged eye closure detected |

---

## 🔍 Functional Workflow

```text
Webcam Input
      │
      ▼
Face Landmark Detection
      │
      ▼
EAR Calculation
MAR Calculation
Gaze Tracking
Head Pose Analysis
      │
      ▼
Driver State Classification
      │
      ▼
Alarm & Visual Warnings
```

---

## 📸 Sample Outputs

* NORMAL
* DROWSY
* MICROSLEEP
* YAWNING DETECTED
* LOOKING LEFT
* LOOKING RIGHT
* HEAD DOWN
* PHONE DISTRACTION

---

## 🎯 Applications

* Advanced Driver Assistance Systems (ADAS)
* Driver Fatigue Monitoring
* Road Safety Systems
* Smart Transportation
* Fleet Monitoring Solutions
* Commercial Vehicle Safety

---

## 🚀 Future Enhancements

* Deep Learning-based Fatigue Detection
* Mobile Phone Detection using YOLO
* Head Pose Estimation using 3D Models
* Face Recognition for Driver Identification
* Cloud-based Monitoring Dashboard
* Email/SMS Emergency Alerts
* Multi-face Monitoring

---

## 📈 Key Learning Outcomes

* Computer Vision Fundamentals
* Real-Time Video Processing
* Facial Landmark Analysis
* Human Behavior Monitoring
* Driver Safety Analytics
* MediaPipe Face Landmarker Integration

---

## 👩‍💻 Author

**Vaka Pujitha**

* MCA Graduate
* Data Science & GenAI Trainee
* Passionate about AI, Machine Learning, Computer Vision, and Data Analytics

---

## ⭐ If you found this project useful, please give it a star on GitHub!

```bash
⭐ Star this repository
🍴 Fork this repository
📢 Share with others
```
