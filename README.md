# DA5401 - Assignment 2: Dimensionality Reduction, Visualization, and Classification


- **Name**: Rishabh Gupta
- **Roll Number**: DA25M024

---

## 📘 Project Overview
This assignment demonstrates the application of **Principal Component Analysis (PCA)** on the **Mushroom Classification dataset** to reduce dimensionality, followed by evaluating how dimensionality reduction impacts the performance of a **Logistic Regression classifier**.

The notebook includes:
1. **Exploratory Data Analysis (EDA) & Preprocessing**  
   - One-hot encoding of categorical features  
   - Standardization of features  
2. **Principal Component Analysis (PCA)**  
   - Scree plot with explained variance ratios  
   - Selection of optimal number of principal components  
   - 2D visualization of classes in reduced space  
3. **Classification with Logistic Regression**  
   - Model trained on original dataset  
   - Model trained on PCA-transformed dataset  
   - Comparison of performance metrics (accuracy, precision, recall, F1-score)  
4. **Insights & Storytelling**  
   - Discussion on trade-offs between dimensionality reduction and performance  

---

## 📊 Dataset Information
- **Name**: Mushroom Classification Dataset  
- **Source**: [Kaggle - Mushroom Classification](https://www.kaggle.com/datasets/uciml/mushroom-classification?resource=download)  
- **Target Variable**: `class`  
  - `e` → Edible  
  - `p` → Poisonous  

The dataset contains only categorical variables, which are transformed via one-hot encoding before applying PCA.  

---

## Insights & Analysis
1. **Feature Efficiency:** PCA successfully identified that 58 components could capture the essential information from original 117 features
2. **Performance Preservation:** Minimal accuracy loss (0.082%) demonstrates PCA's effectiveness in preserving discriminatory information
3. **Visual Clarity:** 2D PCA projections revealed meaningful class separation patterns
4. **Computational Benefits:** 50% feature reduction enables faster training and inference

---

## Tech Stack
- Python 3.7+
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- Jupyter Notebook
