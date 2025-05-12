# 🧠 Hyper-Personalized Product Recommendation Engine with Emotion Detection

This repository presents an Orange-based machine learning workflow to create a **Hyper-Personalized Product Recommendation System** enhanced with **Emotion Detection** using both **textual reviews** and **product images**.

## 📌 Project Overview

Conventional recommendation engines lack emotional intelligence and often provide irrelevant suggestions. This project integrates sentiment/emotion detection from reviews with product image embeddings to offer recommendations based on the user’s emotional context.

## 📅 Project Duration

**08-02-2025** to **12-02-2025**

## 👨‍💻 Author

**Abdul Zuhail M**  
*Data Intelligence Research Lab – Quantum Wolf*

---

## 📁 Dataset Overview

### 📝 Text Reviews  
- **File**: `Amazon-Product-Reviews-Sentiment-Analysis-in-Python-Dataset.csv`  
- **Description**: Contains product reviews used for sentiment and emotion detection.  
- **Fields**: `reviewText`, `overall`, `summary`, `emotion_label` (added/augmented)

### 🖼️ Product Images  
- **File**: `filtered_dataset_25.zip`  
- **Structure**:
```bash
filtered_dataset_25/
├── train/
│   ├── class1/
│   ├── class2/
│   └── ...
└── test/
    ├── class1/
    ├── class2/
    └── ...
. Description: Contains product images organized by categories for training and testing visual models.
🔧 Tools & Technologies
| Tool/Technique     | Purpose                                       |
| ------------------ | --------------------------------------------- |
| Orange Data Mining | Workflow creation and visual ML pipelines     |
| Sentiment Analysis | Emotion detection from user reviews           |
| Image Embedding    | Extract image features via pre-trained CNN    |
| PCA                | Reduce feature dimensionality                 |
| K-Means            | Group products/users based on patterns        |
| SVM                | Predict personalized product labels           |
| Visualizations     | Understand predictions and emotional clusters |

🔄 Orange Workflow Summary

🟧 1. Text-Based Emotion Detection

.Widgets: File → Corpus → Preprocess Text → Sentiment Analysis → Data Table
.Goal: Classify emotional tone from review text

🟨 2. Image-Based Feature Embedding

.Widgets: Import Images → Image Embedding → Edit Domain
.Goal: Represent products visually using CNN features

🔵 3. Dimensionality Reduction

.Widgets: PCA
.Goal: Compress image features for efficient learning

🟠 4. Classification and Clustering

.Widgets: Merge Data → K-Means → SVM
.Goal: Combine emotion + image to recommend products

🔮 5. Evaluation and Visualization

.Widgets: Predictions → Confusion Matrix, Box Plot, Scatter Plot
.Goal: View accuracy, cluster groups, emotion-product mapping

🧪 Results
.🎯 Emotionally aligned recommendations
.📊 High-accuracy classification using SVM
.📈 Visualization of clusters and predictions
.📦 Image and text synergy improves recommendation precision

📉 Challenges and Fixes

| Issue                   | Solution                                |
| ----------------------- | --------------------------------------- |
| Large image features    | PCA to reduce dimensionality            |
| Sparse emotion labels   | Added synthetic/emotion-augmented data  |
| Multi-modal data fusion | Used SVM for cross-modal classification |
| Orange’s flexibility    | Used Python scripting inside Orange     |

🚀 Future Enhancements
.Add facial or voice-based real-time emotion input
.Build API for integration with e-commerce platforms
.Deploy via web dashboard or mobile recommendation app
.Real-time recommendation engine with streaming input
