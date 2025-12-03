# 🩺 Skin Disease Detection using Hybrid Deep Learning 

This repository contains our project on **multi-class Skin Disease Detection** using a **Hybrid CNN architecture**, **Out-of-Distribution (OOD) Detection**, and **Explainable AI (Grad-CAM)**.

The model combines the strengths of **ResNet50** (global feature extraction)** and **DenseNet121 (fine-grained texture extraction)** to achieve significantly better accuracy than single-backbone networks.

---

## 🚀 Features

### ✅ **Hybrid Model (ResNet50 + DenseNet121)**
* Parallel feature extraction pipelines  
* Feature fusion for richer representation  
* Improved generalization and accuracy  

---

### ✅ **Multi-Class Skin Disease Classification**
* **22 disease classes**
* **15,000+ real clinical images**
* Softmax-based multi-class prediction  

---

### ✅ **Out-of-Distribution (OOD) Detection**
* Detects unseen or irrelevant images  
* Distance-based novelty identification  
* Prevents unsafe or misleading predictions  

---

### ✅ **Explainability (Grad-CAM)**
* Highlights important lesion regions  
* Improves clinical interpretability  
* Increases model trust and transparency  

---

### ✅ **Baseline Comparison**
* **ResNet50**
* **DenseNet121**
* **PCA-based dimension reduction experiments**

**Hybrid model achieves the highest accuracy: 79.11%**

---

## 📊 Results Summary

| Rank | Model                          | Test Accuracy (%) |
|------|--------------------------------|-------------------|
| 1    | **Hybrid (ResNet50 + DenseNet121)** | **79.11**          |
| 2    | DenseNet121                    | 76.20             |
| 3    | ResNet50                       | 64.88             |

*Training Accuracy:* **97.5%**  
*Testing Accuracy:* **79.11%**

---

## 📁 Dataset

We use the publicly available **Skin Disease Dataset** from Kaggle:

🔗 **https://www.kaggle.com/datasets/pacificrm/skindiseasedataset**

**Dataset Details:**
* 22 skin disease classes  
* ~15,000 images  
* Real-world distribution  
* Class imbalance handled through augmentation  

---

## 🧠 Model Architecture
Input Image
│
├──► ResNet50 Backbone ─────► Feature Vector (Global Features)
│
├──► DenseNet121 Backbone ─► Feature Vector (Texture Features)
│
└──► Feature Fusion ────────► Classification Head ─────► Softmax Output (22 Classes)

