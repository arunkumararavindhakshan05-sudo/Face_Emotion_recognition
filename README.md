# 😊 Real-Time Face Emotion Recognition using OpenCV

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=OpenCV&logoColor=white)
![DeepLearning](https://img.shields.io/badge/Deep_Learning-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

A real-time **facial emotion recognition** system that detects human emotions from a live webcam feed. The system classifies emotions into 7 categories: **Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral**.

---

## 📸 Demo

```
[Live Webcam Feed]
  → Face detected using Haar Cascade
  → Face region cropped and preprocessed
  → Emotion classified by deep learning model
  → Emotion label displayed above bounding box
  
  Output: "Happy 94%" | "Neutral 87%" | "Sad 76%"
```

---

## ⚙️ How It Works

1. **Face Detection** — Haar Cascade detects the face region in each frame
2. **ROI Extraction** — The face region of interest (ROI) is cropped and resized to 48×48 pixels
3. **Grayscale Conversion** — Face ROI is converted to grayscale for model input
4. **Emotion Classification** — A pre-trained CNN model predicts the emotion with confidence score
5. **Label Overlay** — Emotion label and confidence percentage are displayed on the live feed

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core programming language |
| OpenCV | Real-time face detection and video stream |
| TensorFlow / Keras | Deep learning model (CNN) for emotion classification |
| NumPy | Array manipulation and preprocessing |
| Haar Cascade XML | Face detection model |

---

## 😄 Emotion Classes

| Label | Description |
|---|---|
| 😠 Angry | Anger expression |
| 🤢 Disgust | Disgust expression |
| 😨 Fear | Fear expression |
| 😊 Happy | Happy / smiling |
| 😢 Sad | Sadness expression |
| 😲 Surprise | Surprised expression |
| 😐 Neutral | No strong emotion |

---

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/arunkumararavindhakshan05-sudo/Face_Emotion_recognition.git
cd Face_Emotion_recognition

# Install dependencies
pip install opencv-python tensorflow keras numpy
```

---

## ▶️ Usage

```bash
python emotion_detection.py
```

**Controls:**
- Press **`Q`** — Quit the camera feed

---

## 📁 Project Structure

```
Face_Emotion_recognition/
│
├── emotion_detection.py              # Main script
├── model/
│   └── emotion_model.h5              # Pre-trained CNN model
├── haarcascade_frontalface_default.xml
└── README.md
```

---

## 🔮 Future Improvements

- [ ] Train on larger dataset (AffectNet, RAF-DB) for better accuracy
- [ ] Add real-time emotion graph over time
- [ ] Build a Streamlit/Flask web app
- [ ] Deploy as a REST API

---

## 👤 Author

**Arunkumar Aravindhakshan**
🔗 [LinkedIn](https://linkedin.com/in/arunkumar-aravindhakshan) | [GitHub](https://github.com/arunkumararavindhakshan05-sudo)
