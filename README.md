# 🔥 Fire Weather Index (FWI) Prediction

Machine learning project predicting Fire Weather Index (FWI) using Ridge and Lasso regression. Includes data preprocessing, model training, evaluation, and deployment with Flask to provide wildfire risk predictions based on meteorological inputs.

---

## 📊 Dataset
- **Source:** Algerian Forest Fires dataset (UCI Machine Learning Repository)
- **Features:**  
  - Meteorological variables: Temperature, Relative Humidity, Wind Speed, Rainfall  
  - Fire indices: FFMC, DMC, ISI, BUI  
- **Target:** Fire Weather Index (FWI)

---

## ⚙️ Workflow
1. **Exploratory Data Analysis (EDA)**  
   - Data cleaning and handling missing values  
   - Feature engineering and scaling  
   - Visualizations to understand correlations  

2. **Model Training**  
   - Ridge Regression (regularization to reduce overfitting)  
   - Lasso Regression (feature selection + regularization)  
   - Hyperparameter tuning with cross‑validation  
   - Evaluation using RMSE and R² metrics  

3. **Deployment**  
   - Flask web application with HTML templates  
   - User inputs weather parameters → model predicts FWI  
   - Comparison of Ridge vs Lasso predictions  

---

## 🚀 How to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/aayushmansingh051/FWI-Predictor.git
   cd FWI-Predictor
          
