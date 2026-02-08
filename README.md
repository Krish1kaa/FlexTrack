# 🏋️ Curl Counter using MediaPipe & OpenCV

This project implements a **real-time bicep curl counter** using **computer vision** techniques. It leverages **MediaPipe Pose** for human pose estimation and **OpenCV** for video processing to track arm movement and count repetitions accurately.

The notebook demonstrates how joint angles can be computed from detected keypoints to identify curl motion phases (up/down) and increment repetition counts accordingly.

---

## 🚀 Features
- Real-time human pose detection
- Elbow joint angle calculation
- Automatic curl repetition counting
- Visual feedback on video frames
- Works with webcam or recorded video input

---

## 🧠 Approach Overview
1. **Pose Estimation**  
   MediaPipe Pose is used to detect body landmarks such as shoulder, elbow, and wrist.

2. **Angle Computation**  
   The angle between shoulder–elbow–wrist is calculated using vector geometry.

3. **State Detection**  
   - Arm extended → **Down** position  
   - Arm contracted → **Up** position  

4. **Repetition Counting**  
   A curl is counted when a full **down → up → down** cycle is completed.

---

## 📂 Project Structure
.
├── CurlCounter.ipynb
└── README.md


---

## 🛠️ Requirements
Install the required dependencies before running the notebook:

```bash
pip install opencv-python mediapipe numpy matplotlib

## ▶️ How to Run

### Clone the repository

git clone https://github.com/Krish1kaa/FlexTrack.git

cd FlexTrack
jupyter notebook CurlCounter.ipynb



