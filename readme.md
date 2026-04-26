# Deepfake Detection using CNN-GRU (Spatio-Temporal Model)

## 📌 Overview

This project implements a deepfake detection system using a hybrid **CNN-GRU architecture** to capture both spatial and temporal features from video data.

The development process was conducted in **Google Colab**, focusing on data preprocessing, model training, and evaluation.
This repository provides the **training notebook and trained model**, while large datasets are hosted externally.

---

## 🧠 Model Architecture

* **CNN (Xception)** for spatial feature extraction
* **GRU** for temporal sequence modeling
* **Input:** sequences of preprocessed video frames (`.npy`)
* **Output:** binary classification (REAL / FAKE)

---

## ⚙️ Project Workflow

1. **Video Processing**

   * Extract frames from videos
   * Perform face detection and cropping

2. **Preprocessing**

   * Convert frames into NumPy arrays (`.npy`)
   * Normalize and prepare sequential data

3. **Model Training**

   * Train CNN-GRU model using preprocessed data
   * Performed in Google Colab

4. **Output**

   * Trained model saved as `.keras` file

---

## 📊 Results

* **Accuracy:** 85%
* **Recall:** 92%
* **AUC:** 0.91

---

## 🧪 Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Google Colab

---

## 👨‍💻 Contribution

* Designed and implemented CNN-GRU model
* Built preprocessing and training pipeline
* Performed model training, tuning, and evaluation

> Web deployment and system integration were developed collaboratively.

---

## 📂 Dataset & Preprocessed Data

Due to size limitations, the dataset and preprocessed `.npy` files are hosted externally:

🔗 https://drive.google.com/drive/folders/1Vpgj8J_jUXLDo8060xNne38pJDeU6KkI

---

## 🤖 Trained Model

The trained model is stored in this repository using **Git LFS**.

📁 Location:

```text
models/deepfake_cnn_gru_model.keras
```

> Note: Git LFS stores large files separately, so the file may appear as a pointer in GitHub.

---

## ▶️ How to Use / Run

### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Open Notebook

```bash
jupyter notebook
```

Then navigate to:

```text
notebooks/Modeldeeptemporal.ipynb
```

### 3. Prepare Data

* Download `.npy` files from Google Drive
* Place them in the appropriate directory (as used in the notebook)

### 4. Run Training / Inference

* Execute all cells in the notebook
* Adjust paths if running locally instead of Google Colab

---

## ⚙️ Load Model Example

```python
from tensorflow.keras.models import load_model

model = load_model("models/deepfake_cnn_gru_model.keras")
```

---

## 📎 Notes

* This project was developed as a final thesis in Computer Engineering
* Training was performed in Google Colab using GPU acceleration
* Ensure all dependencies are installed before running the notebook
* Update file paths when running outside Colab environment

---
