# APR-Assignment-_1-LR

# 🎬 Movie Collection Success Analysis  

This project analyzes the **Movie_collection_train.csv** dataset to predict whether a movie will be a commercial success.  
The workflow includes **data preprocessing, visualization, dimensionality reduction using LDA, logistic regression modeling, and evaluation**.  

---

## 📌 Project Overview
- Loaded and explored the dataset (400 rows × 19 columns).  
- Handled missing values (`Time_taken`) and dropped redundant columns (`MPAA_film_rating`).  
- Encoded categorical variables (`Genre`, `3D_available`).  
- Created a binary target variable: `Collection_Success` (above-median collection = success).  
- Scaled numerical features for model consistency.  

---

## 🔍 Data Insights
- Target variable distribution was **relatively balanced**.  
- Features such as **Trailer_views, Budget, and 3D_available** showed strong influence on success.  
- Visualization with histograms, box plots, and scatter plots helped reveal trends.  

---

## 📉 Dimensionality Reduction (LDA)
- Applied **Linear Discriminant Analysis (LDA)** to reduce the dataset to **1 discriminant component**.  
- LDA maximized class separability before feeding data into Logistic Regression.  

---

## 🤖 Model & Results
- Model: **Logistic Regression (on LDA-transformed data)**  
- **Accuracy**: 0.8625  
- **Precision**: 0.8718  
- **Recall**: 0.8500  
- **F1-score**: 0.8608  

The logistic regression coefficient for the LDA component was **+2.04**, showing a strong positive relationship with collection success.  

---

## 📈 Key Takeaways
- Logistic Regression + LDA is effective for predicting movie success.  
- Important predictors: **Trailer_views, Budget, 3D_available**.  
- The approach balances **performance and interpretability**.  

---

## 🚀 Future Improvements
- Experiment with **ensemble methods** (Random Forest, XGBoost).  
- Incorporate **textual/social media features**.  
- Test on **larger and more diverse datasets**.  

---

## 🛠️ Tech Stack
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)  
- Machine Learning: **Logistic Regression, LDA**  

---

