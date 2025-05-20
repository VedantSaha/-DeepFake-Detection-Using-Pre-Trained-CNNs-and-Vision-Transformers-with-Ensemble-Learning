# 🎭 DeepFake Detection Using Pre-Trained CNNs and Vision Transformers with Ensemble Learning

This repository contains the LaTeX source code and supplementary assets for a research project focused on detecting DeepFake images using a range of pre-trained deep learning models, including Convolutional Neural Networks (CNNs) and Vision Transformers (ViTs). The project investigates individual model performance, ensemble strategies, and architectural behaviors in data-limited scenarios.

---

## 📄 Project Overview

DeepFakes present a significant challenge to digital media authenticity. This study evaluates the effectiveness of pre-trained CNNs and ViTs on a subset of the **FaceForensics++** dataset for **binary classification** (real vs. fake facial images). Special emphasis is placed on:
- How each architecture handles **limited training data**
- Comparative performance across models
- Benefits of **ensemble learning** for boosting prediction stability

---

## 🧠 Key Models Explored

- **VGG16** — Traditional CNN baseline  
- **Vision Transformer (ViT)** — Transformer-based image classification  
- **GenConViT** — Hybrid CNN-Transformer model  
- **DeepFake-Adapter** — Adapter-based fine-tuning for DeepFake detection  

---

## 🧪 Methodology

- **Dataset:** 200 images from FaceForensics++ (100 real, 100 fake)  
- **Image Dimensions:** 128×128  
- **Preprocessing:** Normalization and minimal augmentation  
- **Training Configuration:**  
  - Binary Cross-Entropy Loss  
  - Adam Optimizer  
  - Early Stopping for generalization  
- **Evaluation Metrics:**  
  - Accuracy  
  - Precision  
  - Recall  
  - F1-score  
- **Ensemble Learning:**  
  - Implemented via soft voting across selected models  

---

## 📊 Results

| Model               | Best Accuracy | Notes                                               |
|---------------------|----------------|------------------------------------------------------|
| VGG16               | **70%**        | Best individual model performance                    |
| Vision Transformer  | Lower          | Underperformed due to data constraints               |
| Ensemble (Soft Vote)| Slightly better| Minor improvement in prediction consistency          |

---

## 📚 References

The project references include:
- **FaceForensics++ dataset**
- **Original VGGNet and Vision Transformer papers**
- **Hugging Face Transformers documentation**
- **Scikit-learn** library for metrics and ensemble implementation


