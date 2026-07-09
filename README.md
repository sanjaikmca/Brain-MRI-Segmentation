# 🧠 Brain MRI Tumor Segmentation using U-Net

> IEEE Published Research Project | Deep Learning | Medical Image Segmentation | TensorFlow | Keras

## 📌 Overview

This project presents an automated **Brain MRI Tumor Segmentation** system using the **U-Net Convolutional Neural Network** architecture. The model accurately identifies and segments tumor regions from brain MRI images, assisting medical professionals in faster and more reliable diagnosis.

The work has been published in an **IEEE Conference**, demonstrating the effectiveness of deep learning techniques for medical image analysis.

---

## 🚀 Features

- 🧠 Automatic Brain Tumor Segmentation
- 📷 MRI Image Preprocessing
- 🔬 U-Net Deep Learning Architecture
- ⚡ TensorFlow & Keras Implementation
- 📊 Dice Loss Optimization
- 📈 Model Training & Validation
- 🎯 Pixel-wise Tumor Mask Prediction
- 📑 IEEE Published Research

---

---

## 📊 Dataset

This project uses the **Brain MRI Images for Brain Tumor Detection and Segmentation** dataset (commonly known as **kaggle_3m**) available on Kaggle.

### Dataset Overview

- **Source:** Kaggle
- **Dataset Name:** Brain MRI Images for Brain Tumor Detection and Segmentation (kaggle_3m)
- **Data Type:** Brain MRI Images with Pixel-wise Tumor Masks
- **Image Format:** `.tif`
- **Mask Format:** `.tif`
- **Task:** Binary Semantic Segmentation

Each MRI image has a corresponding **ground truth mask** where:

- **White pixels (1):** Tumor Region
- **Black pixels (0):** Background

---

### Dataset Structure

```
kaggle_3m/
│
├── Patient_001/
│   ├── image_1.tif
│   ├── image_1_mask.tif
│   ├── image_2.tif
│   ├── image_2_mask.tif
│   └── ...
│
├── Patient_002/
│   ├── ...
│
└── ...
```

---

### Data Preprocessing

Before training the U-Net model, the following preprocessing steps were performed:

- Converted MRI images to grayscale
- Resized images to **128 × 128**
- Normalized pixel values to the range **[0, 1]**
- Loaded corresponding tumor masks
- Created image-mask pairs for supervised learning

---

### Input and Output

| Input | Output |
|--------|---------|
| Brain MRI Image | Tumor Segmentation Mask |

The model learns to predict the tumor region for each MRI image by generating a pixel-level segmentation mask.

---

### Dataset Link

📌 Kaggle:
https://www.kaggle.com/datasets/mateuszbuda/lgg-mri-segmentation

---

## 🏗️ Model Architecture

The project uses the **U-Net** architecture consisting of:

- Encoder (Contracting Path)
- Bottleneck Layer
- Decoder (Expanding Path)
- Skip Connections
- Sigmoid Output Layer

The network performs semantic segmentation to classify every pixel as either:

- Tumor
- Background

---

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib
- Google Colab

---

## 📂 Project Structure

```
Brain-MRI-Segmentation/
│
├── brain_research.ipynb
├── dataset/
├── trained_model/
├── results/
├── images/
└── README.md
```

---

## 📊 Training Details

| Parameter | Value |
|-----------|-------|
| Input Size | 128 × 128 |
| Optimizer | Adam |
| Loss Function | Dice Loss |
| Output Activation | Sigmoid |
| Batch Size | 16 |
| Epochs | 20 |

---

## 📈 Evaluation

The model is evaluated using segmentation performance metrics such as:

- Dice Score
- Intersection over Union (IoU)
- Accuracy

These metrics measure how accurately the predicted tumor region overlaps with the ground truth mask.

---

## 💻 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Brain-MRI-Segmentation.git
```

Move into the project

```bash
cd Brain-MRI-Segmentation
```

Install dependencies

```bash
pip install tensorflow opencv-python matplotlib numpy
```

Run the notebook using Jupyter Notebook or Google Colab.

---

## Workflow

```
Brain MRI Image
        │
        ▼
Image Preprocessing
        │
        ▼
U-Net Model
        │
        ▼
Tumor Segmentation Mask
        │
        ▼
Performance Evaluation
```

---

## 🎯 Applications

- Brain Tumor Detection
- Medical Image Analysis
- Clinical Decision Support
- Radiology Assistance
- AI-assisted Healthcare

---

## 📄 Research Publication

This project is based on my **IEEE Published Research Paper** in the field of **Medical Image Segmentation using Deep Learning**.

📚 **Publication:** IEEE Conference Paper

*https://doi.org/10.1109/ICCRTEE68719.2026.11566521*

---

## 👨‍💻 Author

**Sanjai K**

MCA Graduate (2026)

IEEE Published Researcher

Machine Learning | Deep Learning | Computer Vision | NLP

GitHub: https://github.com/sanjaikmca

LinkedIn: *https://www.linkedin.com/in/sanjaikmca*

---

## ⭐ If you found this project useful

Please consider giving it a ⭐ on GitHub!
