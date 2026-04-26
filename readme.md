# Deepfake Detection using CNN-GRU (Spatio-Temporal Model)

## 📌 Overview
This project implements a deepfake detection system using a hybrid CNN-GRU architecture to analyze spatial and temporal features from video frames.

This repository focuses on **model development and training pipeline**.  
The full system (including web deployment and multi-model integration) was developed collaboratively.

---

## 🧠 Model Architecture
- CNN (Xception) for spatial feature extraction  
- GRU for temporal sequence modeling  
- Input: video frames  
- Output: REAL / FAKE classification  

---

## ⚙️ Features
- Video frame extraction  
- Face detection & cropping  
- Image preprocessing  
- Deep learning model training  
- Model evaluation using standard metrics  

---

## 📊 Results
- Accuracy: 85%  
- Recall: 92%  
- AUC: 0.91  

---

## 🧪 Tech Stack
- Python  
- TensorFlow / Keras  
- OpenCV  
- NumPy  

---

## 👨‍💻 My Contribution
- Developed CNN-GRU deep learning model  
- Built preprocessing and training pipeline  
- Performed model training, tuning, and evaluation  

> Web deployment and system integration were handled collaboratively with team members.

---

## 📂 Dataset & Preprocessed Data
Due to size limitations, dataset and preprocessed files are hosted externally:

🔗 https://drive.google.com/drive/folders/1Vpgj8J_jUXLDo8060xNne38pJDeU6KkI

---

## 🤖 Trained Model
The trained model is included in this repository using Git LFS.

Available formats:
- `deepfake_cnn_gru_model.keras`  
- `deepfake_cnn_gru_model.weights.h5` 

---

## ▶️ How to Run
```bash
pip install -r requirements.txt
python src/train.py
```

---

## ⚙️ Load Model Example
```python
from tensorflow.keras.models import load_model

model = load_model("deepfake_cnn_gru_model.keras")
```

---

## 📎 Notes
This project was developed as a final thesis project in Computer Engineering.
