# 🍷 Wine Quality Classification

## 📌 Project Description
The Wine Quality Classification project predicts the quality of red wine based on its chemical properties such as acidity, pH, and alcohol content. 
The dataset originally provides quality scores from 3-8, but these were grouped into three categories: Low (3–4), Medium (5–6), and High (7–8), 
turning it into a classification problem.

### Workflow
1. **Data Cleaning** – Removed duplicates and checked for missing values.
2. **EDA** – Explored feature distributions, correlations, and outliers.
3. **Multicollinearity Check** – Detected high correlation between `fixed acidity` and `density` using VIF.
4. **PCA** – Reduced multicollinearity by combining correlated features into a single principal component (`acidity_density_PC`).
5. **Data Splitting** – Train-test split (70:30 ratio).
6. **Encoding** – Converted target labels (Low, Medium, High) into numeric values using Ordinal Encoding.
7. **Balancing Classes** – Applied SMOTE to handle class imbalance and prevent bias toward majority class.
8. **Model Training** – Trained a Random Forest Classifier for prediction.
9. **Evaluation** – Evaluated the model using accuracy, precision, recall, F1-score, confusion matrix, and ROC curves.
9. **Tuning** – Tuned Model using grid_search_cv.

### Key Learnings
- Importance of preprocessing and handling class imbalance.
- Using PCA to reduce multicollinearity.
- Application of Random Forest for robust classification.

### Applications
This model can assist wineries, quality control labs, and consumer recommendation systems in predicting wine quality efficiently.

---

## ▶️ How to Run
1. Clone the repository and navigate into the project folder.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook Classification.ipynb
   ```

