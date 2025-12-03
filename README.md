🩺 Skin Disease Detection using Hybrid Deep Learning (ResNet50 + DenseNet121)

This repository contains our Foundations of Machine Learning (AI60203) project on multi-class Skin Disease Detection using a Hybrid CNN architecture, Out-of-Distribution (OOD) Detection, and Explainable AI (Grad-CAM).

The model combines the strengths of ResNet50 (global features) and DenseNet121 (fine-grained textures) to achieve significantly better accuracy than single-backbone networks.

🚀 Features
✅ Hybrid Model (ResNet50 + DenseNet121)

Parallel feature extraction pipelines

Feature fusion for richer representation

Improved generalization and accuracy

✅ Multi-Class Skin Disease Classification

22 disease classes

Dataset with 15,000+ real clinical images

Softmax-based multi-class prediction

✅ Out-of-Distribution (OOD) Detection

Detects unseen or irrelevant images

Distance-based novelty identification

Prevents unsafe or misleading predictions

✅ Explainability (Grad-CAM)

Highlights important regions in images

Helps in clinical interpretability

Increases model trust and transparency

✅ Baseline Comparison

ResNet50

DenseNet121

PCA-based dimensionality reduction tests

Hybrid model achieves the highest test accuracy: 79.11%

📊 Results Summary
Rank	Model	Test Accuracy (%)
1	Hybrid (ResNet50 + DenseNet121)	79.11
2	DenseNet121	76.20
3	ResNet50	64.88

Training Accuracy: 97.5%
Testing Accuracy: 79.11%

📁 Dataset

We use the publicly available Skin Disease Dataset from Kaggle:

🔗 https://www.kaggle.com/datasets/pacificrm/skindiseasedataset

22 skin disease classes

~15,000 images

Real-world clinical distribution

Imbalanced dataset (handled via augmentation)
Input Image
     │
     ├──► ResNet50 Backbone ──► Feature Vector (Global Features)
     │
     ├──► DenseNet121 Backbone ─► Feature Vector (Texture Features)
     │
     └──► Feature Fusion ───► Classification Head ───► Softmax Output (22 Classes)
