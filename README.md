# 🖋️ Handwritten Digit Recognition WebApp

![Project Banner](frontend/static/images/banner.png)

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.13.0-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)
[![Flask](https://img.shields.io/badge/Flask-2.0.1-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Vercel](https://img.shields.io/badge/Vercel-Deployed-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/)

A sophisticated web-based application that recognizes handwritten digits (0-9) using a deep Convolutional Neural Network (CNN). This project seamlessly integrates modern web aesthetics with powerful machine learning to provide a real-time, interactive experience.

## 🚀 Key Features

- **Interactive Canvas:** Draw digits directly in your browser with smooth, responsive stroke rendering.
- **Real-time Prediction:** Get instant classification results with high confidence scores.
- **Glassmorphism UI:** A sleek, modern interface built with premium design principles.
- **Advanced CNN Architecture:** Utilizes residual connections and data augmentation for 99%+ accuracy.
- **Mobile Responsive:** Works perfectly on desktops, tablets, and smartphones.

## 🛠️ Tech Stack

- **Frontend:** HTML5 Canvas, Vanilla CSS (Glassmorphism), JavaScript (ES6+).
- **Backend:** Python Flask API, NumPy, Pillow.
- **Machine Learning:** TensorFlow/Keras, CNN with Residual Blocks.
- **Deployment:** Optimized for Vercel and local hosting.

## 🧠 Neural Network Architecture

The heart of this application is a custom-designed CNN inspired by ResNet architectures:

- **Input:** 28x28x1 Grayscale.
- **Convolutional Blocks:** 3 blocks with Dual Conv2D layers, Batch Normalization, and **Residual Connections**.
- **Regularization:** Dropout (0.25 - 0.5) and Batch Normalization at every stage to prevent overfitting.
- **Dense Layers:** 512 and 256 units with ReLU, leading to a 10-unit Softmax output.

## 📁 Project Structure

```text
HandWritten_Digit_Recognition_WebApp/
├── backend/
│   ├── api/
│   │   └── app.py            # Flask API & Endpoints
│   └── model/
│       ├── digit_model.h5    # Trained Weights
│       └── train_model.py    # Training Script & Architecture
├── frontend/
│   ├── static/
│   │   ├── css/ style.css    # Premium Glassmorphism Design
│   │   ├── js/ script.js     # Canvas Logic & API Calls
│   │   └── images/           # Assets & Banners
│   └── templates/
│       └── index.html        # Main Entry Page
├── requirements.txt          # Python Dependencies
└── vercel.json               # Vercel Deployment Config
```

## ⚙️ Installation & Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Mujtabanite/HandWritten_Digit_Recognition_WebApp.git
   cd HandWritten_Digit_Recognition_WebApp
   ```

2. **Set up Virtual Environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the App:**
   ```bash
   python backend/api/app.py
   ```

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
Developed with ❤️ by [Mujtabanite](https://github.com/Mujtabanite)
