# ❤️ Heart Disease Prediction using Clustering Regression

A machine learning project focused on identifying high-risk individuals for heart disease through interpretable clustering and predictive modeling.

## 📌 Project Objective

Heart disease is the leading cause of death worldwide. Early detection can save lives and reduce healthcare costs. Our objective is to create interpretable profiles that help physicians identify high-risk individuals by:

- Clustering patients based on key clinical features.
- Predicting heart disease likelihood using logistic regression within each cluster.
- Providing actionable insights for early intervention.

## 🧠 Methods

This project combines unsupervised and supervised learning techniques:

1. **Feature Selection**  
   - Used a Classification Tree to select the most predictive features.
   - Achieved balanced accuracy, precision, recall, and F1-score of 0.86.

2. **Clustering Approaches**  
   - **Gaussian Mixture Models (GMM)**: Selected as final model for its clear separation into high and low risk clusters.
   - **Latent Class Analysis (LCA)**: Required binning of numeric features.
   - **K-Prototype Clustering**: Handled mixed categorical and numerical data.

3. **Within-Cluster Regression**  
   - Logistic Regression used to estimate probability of heart disease within each cluster.
   - Classification Tree also tested as a comparative model.

## 🧾 Dataset

- Source: [UCI Heart Disease Dataset](https://archive.ics.uci.edu/dataset/45/heart+disease)
- Features: 13 clinical attributes (e.g., age, sex, chest pain type, cholesterol)
- Target: Presence (`1`) or absence (`0`) of heart disease

## 🧪 Model Evaluation

| Model                | Training Accuracy | Testing Accuracy |
|---------------------|-------------------|------------------|
| Classification Tree + GMM | 0.91              | 0.73             |
| Logistic Regression + GMM | 0.88              | **0.87**         |

- **Key Metric: Relative Risk (RR)**  
  - High-risk cluster (C1) patients are **4.4x** more likely to develop heart disease than those in the low-risk cluster.

## ✅ Final Model: Logistic Regression + Gaussian Mixture Clustering

- Chosen for its high interpretability and strong performance.
- RR and predictive probabilities closely match empirical distributions.
- Practical for physicians to implement as a red-flag system.

## 🔍 Future Work

- Incorporate patient lifestyle traits (e.g., smoking, physical activity).
- Expand the training dataset for improved generalizability.
- Develop an interactive dashboard for physicians.

## 📁 Project Structure
📦 HeartDiseasePrediction/ ├── Predicting-Heart-Disease.ipynb ├── README.md └── presentation.pdf

## 🧑‍💻 Team

- Hyunji Amy Kim
- Zhiwei Guo
- Samuel Martinez Koss
- Alvin Yao

## 📜 License

This project is for educational purposes and not intended for clinical use.

---

> *“The machine never stops learning.”*
