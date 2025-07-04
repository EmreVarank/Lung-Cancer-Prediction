# 🩺 Early Stage Lung Cancer Prediction Using Machine Learning

This project aims to build reliable machine learning models for the early prediction of lung cancer based on clinical symptoms and demographic data. It also compares multiple algorithms to identify the most accurate and balanced classifier, especially minimizing **false negatives**, which are critical in healthcare. For detailed analysis and results, please see `Documents/VeriMadenciligiFinal.docx`. For a video overview of the project: https://youtu.be/lhrUXwT5a5U?si=w0bwMZ2RvXimHGX7.

---

## 📂 Project Structure

- `Database/`: Includes the dataset (`lung_cancer.csv`)
- `Documents/`: Contains documentation reports and references
- `Python/main.pynb`: All Python scripts for preprocessing, modeling, and evaluation

---

## 🎯 Objectives

- Develop ML models to classify whether a person has lung cancer
- Analyze the performance of each algorithm
- Focus on minimizing false negatives in predictions

---

## 📊 Dataset Overview

- Source: [Kaggle - Lung Cancer Dataset](https://www.kaggle.com/datasets/mysarahmadbhat/lung-cancer/data)
- Features: Age, Gender, Smoking, Fatigue, Shortness of Breath, etc.
- Target: `LUNG_CANCER` (0 = No, 1 = Yes)

---

## ⚙️ Machine Learning Models Used

- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**
- **Random Forest (RF)**
- **Voting Classifier (SVM + KNN + RF)**

---

## 📈 Key Results

| Model              | Accuracy | Recall (Cancer) | FN | FP | Note |
|--------------------|----------|------------------|----|----|------|
| SVM (Linear)       | 92.8%    | 0.94             | 3  | 1  | Balanced and strong |
| KNN (k=2)          | 92.8%    | 0.92             | 4  | 0  | No FP, but FN ↑     |
| Random Forest      | 92.8%    | 0.96             | 2  | 2  | Stable performance  |
| **Voting Classifier** | **94.6%** | **0.98**        | **1**| 2 | **Best overall**    |

---

## 🧪 Visuals & Insights

- Heatmaps for feature correlation
- Class distribution plots (gender, age, smoking status)
- Confusion matrices for all models
- Precision, Recall, F1-score evaluations

---

## 📄 Documentation

- 📘 `Documents/VeriMadenciliğiFinal.docx`: Detailed project write-up
- 📗 `Documents/Early_Stage_Lung_Cancer_Prediction_Using_Various_Machine_Learning_Techniques.pdf`: Source publication reference

---

## ⚙️ How to Run 

Follow the steps below to set up and run the project on your local machine:

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/EmreVarank/Lung-Cancer-Prediction.git
cd Lung-Cancer-Prediction
```

### 2️⃣ Install Required Libraries

Make sure you have Python 3.7+ installed. Then, install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3️⃣ Run the Project

Navigate to the Python folder and run the main script:

```bash
cd Python
python main.py
```


