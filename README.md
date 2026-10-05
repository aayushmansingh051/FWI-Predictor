# 🔥 Fire Weather Index (FWI) Prediction

An end-to-end **Machine Learning web application** that predicts the **Fire Weather Index (FWI)** using meteorological and fire-weather parameters. The project covers data preprocessing, feature engineering, regression modeling, hyperparameter tuning, model evaluation, and deployment through a Flask web application.

🌐 **Live Demo:** https://fwi-predictor-ktty.onrender.com/predictdata

💻 **GitHub Repository:** https://github.com/aayushmansingh051/FWI-Predictor

---

## 📌 Project Overview

The **Fire Weather Index (FWI)** is a numerical indicator used to represent fire danger based on weather and environmental conditions.

This project uses Machine Learning to predict FWI from relevant meteorological and fire-weather parameters. A Flask-based web application provides a simple interface where users can enter the required values and receive an FWI prediction.

The project demonstrates a complete **Machine Learning lifecycle**, from data preprocessing and model training to web deployment.

---

## 🎯 Objectives

* Predict Fire Weather Index using Machine Learning
* Perform data cleaning and preprocessing
* Apply feature engineering and feature scaling
* Train and compare regression models
* Perform hyperparameter tuning using cross-validation
* Evaluate model performance using R² and RMSE
* Serialize trained models
* Build a reusable prediction pipeline
* Develop a Flask-based web application
* Deploy the application online

---

## ✨ Features

* 🔥 Fire Weather Index prediction
* 📊 Exploratory Data Analysis
* 🧹 Data cleaning and preprocessing
* ⚙️ Feature engineering and scaling
* 🤖 Ridge Regression
* 🤖 Lasso Regression
* 🔍 Hyperparameter tuning
* 🔄 Cross-validation
* 📈 Model evaluation using R² and RMSE
* 💾 Model serialization
* 🌐 Flask web application
* ☁️ Cloud deployment using Render

---

## 📊 Dataset

The project uses the **Algerian Forest Fires Dataset**, which contains meteorological measurements and fire-weather indices.

### Input Features

* **Temperature**
* **Relative Humidity (RH)**
* **Wind Speed (Ws)**
* **Rain**
* **Fine Fuel Moisture Code (FFMC)**
* **Duff Moisture Code (DMC)**
* **Initial Spread Index (ISI)**
* **Buildup Index (BUI)**

### Target Variable

* **Fire Weather Index (FWI)**

---

## 🧠 Machine Learning Workflow

```text
Raw Dataset
     ↓
Data Cleaning
     ↓
Exploratory Data Analysis
     ↓
Feature Engineering
     ↓
Feature Scaling
     ↓
Train-Test Split
     ↓
Model Training
     ↓
Cross-Validation
     ↓
Hyperparameter Tuning
     ↓
Model Evaluation
     ↓
Best Model Selection
     ↓
Model Serialization
     ↓
Prediction Pipeline
     ↓
Flask Web Application
     ↓
Cloud Deployment
```

---

## 🤖 Machine Learning Models

### Ridge Regression

Ridge Regression uses **L2 regularization** to reduce the impact of large coefficients and help minimize overfitting.

### Lasso Regression

Lasso Regression uses **L1 regularization**, which can reduce less important feature coefficients toward zero and perform feature selection.

Both models are evaluated and compared to determine the better-performing model for FWI prediction.

---

## 🔬 Model Evaluation

The models are evaluated using standard regression metrics.

| Metric       | Description                                                                                |
| ------------ | ------------------------------------------------------------------------------------------ |
| **R² Score** | Measures how well the model explains the variance in the target variable                   |
| **RMSE**     | Measures the average magnitude of prediction error, giving greater weight to larger errors |

### Model Performance

| Model            | R² Score | RMSE |
| ---------------- | -------: | ---: |
| Ridge Regression |        — |    — |
| Lasso Regression |        — |    — |

> Model scores can be added after the final training run.

---

## 🌐 Web Application

The project includes a **Flask-based web application** that allows users to enter meteorological parameters and obtain an FWI prediction.

### Prediction Flow

```text
User Input
    ↓
Flask Application
    ↓
Input Processing
    ↓
Feature Transformation
    ↓
Trained ML Model
    ↓
FWI Prediction
    ↓
Result Displayed
```

### 🚀 Live Application

**[Open FWI Predictor](https://fwi-predictor-ktty.onrender.com/predictdata)**

---

## 📂 Project Structure

```text
FWI-Predictor/
│
├── artifacts/
│   ├── model.pkl
│   └── preprocessor.pkl
│
├── notebook/
│   ├── EDA
│   └── Model Training
│
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/
│   │   ├── predict_pipeline.py
│   │   └── train_pipeline.py
│   │
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── templates/
│   ├── index.html
│   └── home.html
│
├── app.py
├── requirements.txt
├── setup.py
├── README.md
└── .gitignore
```

---

## 🛠️ Tech Stack

### Programming Language

* Python

### Machine Learning

* Scikit-learn
* Pandas
* NumPy

### Data Analysis & Visualization

* Matplotlib
* Seaborn
* Jupyter Notebook

### Web Development

* Flask
* HTML
* CSS
* JavaScript

### Deployment

* Gunicorn
* Render

### Version Control

* Git
* GitHub

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/aayushmansingh051/FWI-Predictor.git
```

### 2. Navigate to the Project

```bash
cd FWI-Predictor
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

#### Windows

```bash
venv\Scripts\activate
```

#### macOS / Linux

```bash
source venv/bin/activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the Application

```bash
python app.py
```

The application will be available at:

```text
http://127.0.0.1:5000/
```

---

## 💾 Model Persistence

The trained Machine Learning model and preprocessing components are serialized and stored as artifacts.

```text
model.pkl
preprocessor.pkl
```

During prediction, these artifacts are loaded by the prediction pipeline so the application can generate predictions without retraining the model.

---

## 🧩 Key Concepts Demonstrated

This project demonstrates practical knowledge of:

* Exploratory Data Analysis (EDA)
* Data Cleaning & Preprocessing
* Feature Engineering
* Feature Scaling
* Train-Test Split
* Regression Modeling
* Regularization
* Model Comparison
* Hyperparameter Tuning
* Cross-Validation
* Model Evaluation
* R² and RMSE Metrics
* Model Serialization
* Prediction Pipeline
* Exception Handling
* Logging
* Flask Web Application
* Machine Learning Deployment
* Git & GitHub

---

## 🔮 Future Improvements

Possible improvements include:

* [ ] Add MAE evaluation
* [ ] Add model performance comparison visualizations
* [ ] Add feature importance visualization
* [ ] Add SHAP-based model explainability
* [ ] Add FWI risk-level classification
* [ ] Add historical FWI trend visualization
* [ ] Add real-time weather API integration
* [ ] Add location-based predictions
* [ ] Add automated model retraining
* [ ] Add model monitoring and drift detection
* [ ] Improve production deployment configuration

---

## 📸 Screenshots

Screenshots of the web application can be added here.

```markdown
![FWI Predictor Home Page](screenshots/home.png)

![FWI Prediction Result](screenshots/result.png)
```

Adding screenshots makes the repository easier for recruiters and other developers to understand.

---

## 🚀 Deployment

The application is deployed using **Render**.

### Deployment Flow

```text
GitHub Repository
       ↓
Render
       ↓
Install Dependencies
       ↓
Start Flask Application
       ↓
Gunicorn
       ↓
Public Web Application
```

### Production Start Command

```bash
gunicorn app:app
```

---

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

* Building an end-to-end Machine Learning project
* Working with real-world weather and fire datasets
* Performing data preprocessing
* Applying feature engineering
* Training regression models
* Using regularization techniques
* Performing hyperparameter tuning
* Using cross-validation
* Evaluating regression models
* Creating reusable prediction pipelines
* Integrating Machine Learning with Flask
* Deploying an ML application to the cloud
* Managing projects using Git and GitHub

---

## 👨‍💻 Author

### Aayushman Singh

**B.Tech — Computer Science & Engineering**
**Specialization — Artificial Intelligence & Machine Learning**
**KIIT University**

🔗 **GitHub:** https://github.com/aayushmansingh051

🔗 **Project Repository:** https://github.com/aayushmansingh051/FWI-Predictor

---

## ⭐ Support

If you found this project useful or interesting, consider giving the repository a ⭐ on GitHub.

---

## 📄 License

This project is developed for educational and portfolio purposes.
