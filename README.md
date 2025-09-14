# Job Placement Prediction – Pathrise (KNN Classifier)

This project focuses on predicting whether a candidate will be successfully placed during the **Pathrise program** using the **K-Nearest Neighbors (KNN)** algorithm.  
The entire implementation and experiments were conducted in **Google Colab**.

---

## 📌 Project Overview
The main research question:  
**Can we predict if a candidate will be placed at Pathrise?**

- **Dataset**: Participant data from the Pathrise program (2,544 individuals, 17 features).  
- **Target**: `placed` → `1` if hired, `0` if not.  
- **Preprocessing**:  
  - Removed irrelevant columns (`cohort_tag`, `pathrise_status`, `number_of_interviews`, `id`).  
  - Converted categorical/object columns to integer values.  
  - Removed very short program durations (< 15 days).  

---

## ⚙️ Model & Methodology
- **Algorithm**: K-Nearest Neighbors (KNN) – chosen for simplicity and interpretability.  
- **Hyperparameter Optimization**:  
  - Tuned `n_neighbors` between 1 and 10.  
  - Used **Grid Search** for optimal parameter selection.  
- **Evaluation Metrics**:  
  - Accuracy  
  - Mean Absolute Error (MAE)  
  - Confusion Matrix  

---

## 🔑 Results
- **Accuracy**: ~74%  
- **MAE Improvement**: Reduced from **26% → 25.5%** after hyperparameter tuning.  
- **Confusion Matrix**: Helped visualize correct vs incorrect classifications across both classes.  

---

## 🚀 How to Run
1. Open the notebook in **Google Colab**.  
2. Upload the dataset (`dataset.csv`).  
