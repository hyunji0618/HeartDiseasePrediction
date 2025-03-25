# Heart Disease Prediction using Clustering Regression

This machine learning project focuses on identifying high-risk individuals for heart disease through clustering and predictive modeling.
📎 **[View Presentation Slides (PDF)](https://github.com/hyunji0618/HeartDiseasePrediction/blob/main/Presentation.pdf)**

## 📌 Project Objective

Heart disease remains the leading cause of death worldwide. In 2022, 702,880 people died from heart disease—equivalent to 1 in every 5 deaths. From 2019 to 2020, heart disease cost about $252.2 billion in healthcare services, medications, and lost productivity.

**Early detection saves lives.**  
Our goal is to build interpretable machine learning profiles to help physicians:

- Cluster patients based on key clinical features
- Predict the likelihood of heart disease using logistic regression within each cluster
- Provide actionable insights for early intervention

## 🧠 Methods

This project combines unsupervised and supervised machine learning techniques:

1. **Feature Selection:**  
   Used a **Classification Tree** to select the most predictive features.
   Achieved balanced accuracy, precision, recall, and F1-score of 0.86.

3. **Clustering Model Selection:**
   Trained and compared multiple clustering models to determine the best approach for regression:
   - **Gaussian Mixture Models (GMM)**
   - **Latent Class Analysis (LCA)**
   - **K-Prototype Clustering**

4. **Within-Cluster Regression:**  
   Using the best clustering method and derived clusters, we trained a **Logistic Regression** model to estimate heart disease probability within each cluster.  
   A **Classification Tree** was also tested as a comparative model.

## 🧾 Dataset

- Source: [UCI Heart Disease Dataset](https://archive.ics.uci.edu/dataset/45/heart+disease)
- Features: 13 clinical attributes (e.g., age, sex, chest pain type, cholesterol)
- Target: Presence (`1`) or absence (`0`) of heart disease

## 🧪 Model Evaluation

| Model                | Training Accuracy | Testing Accuracy |
|---------------------|-------------------|------------------|
| Classification Tree + GMM | 0.91              | 0.73             |
| Logistic Regression + GMM | 0.88              | **0.87**         |


## ✅ Conclusion

### Final Model: Logistic Regression + Gaussian Mixture Clustering

- Chosen for its **strong performance** and **interpretability**
- Allows calculation of **Relative Risk (RR)**
- Predictive probabilities aligned with empirical proportions
- Practical as a red-flag system for use in healthcare

**Key Metric: Relative Risk (RR)**  
Patients in the **high-risk cluster (C1)** are **4.4x** more likely to develop heart disease than those in the **low-risk cluster (C0)**.
    
## 🔍 Future Work

- Incorporate lifestyle features (e.g., smoking, exercise, diet)
- Expand training dataset to improve generalizability
- Develop an interactive dashboard for clinical deployment
  
## 🧑‍💻 Team

- Hyunji Amy Kim
- Zhiwei Guo
- Samuel Martinez Koss
- Alvin Yao

## 📜 License

This project is for educational purposes and not intended for clinical use.

---

> *“The machine never stops learning.”*
