# 🧠 Brain Tumor Classification & Explainable AI from MRI

## 📌 Overview

This project presents a **comprehensive Computer Vision + Deep Learning framework** for detecting and classifying brain tumors from MRI scans.

The system classifies images into:

* Glioma
* Meningioma
* Pituitary Tumor
* No Tumor

Along with prediction, it provides **Explainable AI insights** using Grad-CAM and detailed **region-based analysis**.

📄 Based on research work: 

---

## 🎯 Key Features

* ✅ MRI Image Preprocessing using CLAHE
* ✅ Transfer Learning with 5 CNN Models:

  * VGG16
  * ResNet50
  * InceptionV3
  * EfficientNetB0
  * DenseNet121
* ✅ Best Model: **InceptionV3 (85.2% Accuracy)**
* ✅ Grad-CAM Visualization (Explainability)
* ✅ Morphological Processing for noise removal
* ✅ Region Analysis:

  * Area
  * Centroid
  * Bounding Box
  * Solidity & Extent
  * Pixel Intensity Stats
* ✅ Interactive Web App using Gradio

---

## 🏗️ Project Architecture

```
Input MRI → Preprocessing → CNN Model → Prediction
                                     ↓
                             Grad-CAM Heatmap
                                     ↓
                          Morphological Refinement
                                     ↓
                         Contour & Region Analysis
                                     ↓
                           Gradio Visualization
```

---

## 🧪 Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy / Pandas
* Matplotlib
* Gradio

---

## 📂 Dataset

* MRI Brain Tumor Dataset (4 classes)
* Preprocessing:

  * CLAHE (Contrast Enhancement)
  * Resizing (224x224)
  * Normalization

---

## ⚙️ Model Details

Transfer learning approach:

* Pretrained on ImageNet
* Frozen base layers
* Custom classifier head:

  * GlobalAveragePooling
  * Dropout (0.5)
  * Dense Softmax Layer

---

## 📊 Results

| Model          | Accuracy   |
| -------------- | ---------- |
| InceptionV3    | **85.20%** |
| DenseNet121    | 83.22%     |
| VGG16          | 72.39%     |
| ResNet50       | 59.19%     |
| EfficientNetB0 | 29.06%     |

---

## 🔍 Explainable AI (XAI)

* Grad-CAM highlights tumor regions
* Helps understand model decisions
* Improves trust in AI predictions

---

## 📈 Region-Based Analysis

After Grad-CAM:

* Extract contours
* Compute:

  * Area
  * Bounding box
  * Centroid
  * Solidity
  * Extent
  * Pixel intensity statistics

---

## 🌐 Gradio Web App

Features:

* Upload MRI Image
* Get Prediction
* Visual Heatmap
* Region Analysis Output

---

## 🚀 How to Run

```bash
git clone https://github.com/your-username/Brain-Tumor-Classification-Explainable-AI.git
cd Brain-Tumor-Classification-Explainable-AI

pip install -r requirements.txt
python app.py
```

---

## 📁 Project Structure

```
├── dataset/
├── models/
├── preprocessing/
├── training/
├── gradcam/
├── app.py
├── requirements.txt
└── README.md
```

---

## 📌 Future Improvements

* Fine-tuning models
* Ensemble learning
* Tumor segmentation (U-Net)
* Multi-modal MRI analysis

---

## 🤝 Contributions

Pull requests are welcome!

---

## 📜 License

MIT License
