# Personalized Skincare and Makeup Recommendation System

## Overview
This project presents an **AI-powered Personalized Skincare and Makeup Recommendation System** that analyzes a user's facial image (selfie) using **Computer Vision and Deep Learning** techniques to recommend suitable skincare and makeup products.

The system extracts key **skin metrics** such as:
- Skin Type (Oily, Dry, Normal)
- Skin Tone (Fitzpatrick Scale)
- Acne Severity (Low, Moderate, Severe)

Based on these metrics, the system recommends skincare products using a **content-based recommendation system with cosine similarity**.

The application uses:
- **React** for the frontend
- **Flask** for the backend
- **TensorFlow/Keras** for machine learning models.

---

# Features
- Skin type detection using **EfficientNet B0**
- Acne severity detection using **CNN**
- Skin tone classification using **HSV & YCbCr color spaces**
- Product recommendation using **cosine similarity**
- Web-based interface for selfie upload
- Personalized skincare suggestions

---

# Model Performance

| Model | Training Accuracy | Validation Accuracy |
|------|------------------|--------------------|
| Skin Type Detection (EfficientNet B0) | ~87% | ~80% |
| Acne Severity Detection (CNN) | ~68% | ~68% |

### Sample Evaluation Metrics

```text
Accuracy       : 83.33 %
F1 Score       : 0.82
Recall         : 0.83
Precision      : 0.84

Confusion Matrix:
[[2 0 0]
 [0 2 1]
 [0 0 1]]
```

---

# Installation

### Clone the repository

```bash
git clone https://github.com/yourusername/Skyn.git
cd Skyn
```

### Create virtual environment

```bash
virtualenv my_env
```

### Activate environment

**Windows**

```bash
my_env\Scripts\activate
```

**Linux / Mac**

```bash
source my_env/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

# Running the Project

Start the Flask backend:

```bash
python app.py
```

Start the React frontend:

```bash
npm start
```

Open the application in your browser.

---

# Project Structure

```text
Skyn/
│
├── Frontend/            # React frontend
├── ML/
│   └── Skin_metrics/
│       ├── Acne/
│       ├── SkinType/
│       └── SkinTone/
│
├── app.py               # Flask backend
├── requirements.txt
└── README.md
```

---

# Future Improvements
- Detect additional skin issues such as pigmentation and wrinkles
- Improve acne detection accuracy with larger datasets
- Add real-time camera detection
- Deploy as a mobile application

---

# Author

Sumeda
Sriprada
Navya Sri

---
