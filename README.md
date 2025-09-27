# Predicted-heart-failure-risk-consumer-behavior-using-Naive-Bayes

This project applies **Naive Bayes (GaussianNB)** to predict whether a consumer will purchase a product based on **Age** and **Estimated Salary**.  

---

### 📌 Steps
1. **Data Import & Preprocessing**
   - Load dataset `Social_Network_Ads.csv`
   - Exploratory Data Analysis (distribution, correlation, visualization)
   - Feature scaling with `StandardScaler`

2. **Model Training**
   - Train-Test split (75% test size)
   - Model: `GaussianNB` (Naive Bayes Theorem)
   - Fit model on training data

3. **Evaluation**
   The Naive Bayes model achieved an **overall accuracy of 88%** on the test dataset (300 samples).  

   - **Class 0 (Did Not Purchase):**  
     The model performed strongly, with **89% precision**, **92% recall**, and an **F1-score of 0.91**.  
     This indicates it was highly reliable in identifying non-buyers, with very few false positives.  

   - **Class 1 (Purchased):**  
     The model achieved **85% precision**, **79% recall**, and an **F1-score of 0.82**.  
     This shows that while it occasionally missed buyers (lower recall), its predictions of purchases were fairly accurate.  

   - **Overall Performance Summary:**  
     - Accuracy: **88%**  
     - Macro Average F1-score: **0.86**  
     - Weighted Average F1-score: **0.88**  

   These results highlight that the model is particularly strong at detecting **non-buyers**, while still maintaining solid performance for detecting **buyers**. Visualizations such as the confusion matrix heatmap, precision-recall curve, and ROC curve provide further confirmation of the model’s reliability.  

4. **Visualization**
   - Decision boundary on training & test sets
   - Prediction example:  
     - Input: `Age=62`, `Salary=88000`  
     - Output: **1 → Consumer will purchase**

---

### 🔧 Libraries Used
- pandas, numpy  
- matplotlib, seaborn  
- scikit-learn  

---

### 📊 Key Insights
- **Age and Estimated Salary** are significant predictors of purchase behavior.  
- Naive Bayes provides a simple yet effective baseline for binary classification with **88% accuracy**.  

---
🚀 *This project demonstrates a complete machine learning workflow (EDA → Preprocessing → Training → Evaluation → Visualization) using Naive Bayes classifier.*
