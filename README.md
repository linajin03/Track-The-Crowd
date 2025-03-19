# 🚆 TTC Train Crowd Detection (In Revision)

## 📌 Project Overview

This project uses **OpenCV** and **YOLOv8** to detect how crowded a Toronto Transit Commission (TTC) train is in real-time. The system:

1. Detects when a train arrives using **motion detection**.
2. Captures an image of the train interior.
3. Runs **YOLOv8** to detect people inside the train. 
4. Classifies the train's crowd level as **Low, Medium-Low, Medium-High or High** or percentage.
5. Sends the crowd level data to a frontend for display.

## 🛠 Tech Stack

| Technology | Purpose                                     |
| ---------- | ------------------------------------------- |
| OpenCV     | Motion detection for train arrival          |
| YOLOv8     | Real-time person detection inside the train |
| Python     | Backend processing and image analysis       |

## 🚀 Installation

### **1️⃣ Install Dependencies**

```bash
pip install ultralytics opencv-python numpy fastapi uvicorn
```

### **2️⃣ Clone the Repository**

```bash
git clone https://github.com/linajin03/ttc-train-crowd-detection.git
cd ttc-train-crowd-detection
```

### **3️⃣ Run the Backend**

```bash
python backend.py
```

## 🎯 How It Works

1. **Train Arrival Detection** - Uses OpenCV to detect motion.
2. **Crowd Estimation** - YOLOv8 counts people inside the train.
3. **Data Transmission** - Sends real-time crowd levels via WebSockets to the frontend.

## 🏗 Future Improvements

- ✅ Train a custom YOLO model for improved accuracy.
- ✅ Deploy to cloud for real-time monitoring.
- ✅ Mobile app integration for real-time updates.

