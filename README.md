**Live Deployment:** https://heart-disease-predictor-bn1d.onrender.com/

---
# ❤️ Heart Disease Prediction using Machine Learning and Flask API

**Name:** Varun Tiwari

**Registration Number:** 23BAI10130

**Application Number:** IN26009673

**Batch Number:** 1A

**Email:** varun.23bai10130@vitbhopal.ac.in

---

## 📌 Project Overview

This project is developed as part of the Machine Learning Deployment Assignment. The objective is to build a Heart Disease Prediction system using Machine Learning, expose the trained model through a Flask REST API, and deploy the application using Render.

The model predicts whether a patient is likely to have heart disease based on various medical parameters such as age, cholesterol level, blood pressure, chest pain type, and other clinical features.

---

# 🎯 Objectives

- Perform data preprocessing and analysis.
- Train a Machine Learning classification model.
- Save the trained model using Joblib.
- Develop a REST API using Flask.
- Deploy the application on Render.
- Host the project on GitHub.

---

# 📂 Project Structure

```
HeartDiseaseDeployment/
│
├── HeartDiseaseDeployment.ipynb   # Complete model training notebook
├── train_model.py                 # Model training script
├── app.py                         # Flask REST API
├── model.pkl                      # Trained Machine Learning model
├── heart.csv                      # Dataset
├── requirements.txt               # Required Python packages
├── README.md                      # Project documentation
```

---

# 📊 Dataset Information

- **Dataset:** Heart Disease Prediction Dataset
- **Target Variable:** `target`

### Input Features

- age
- sex
- cp
- trestbps
- chol
- fbs
- restecg
- thalach
- exang
- oldpeak
- slope
- ca
- thal

### Output

- **0** → No Heart Disease
- **1** → Heart Disease

---

# 🧠 Machine Learning Model

The project uses a **Random Forest Classifier** from Scikit-learn.

### Why Random Forest?

- High prediction accuracy
- Handles non-linear relationships
- Less prone to overfitting
- Works well with tabular medical datasets

---

# 🛠 Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Flask
- Joblib
- GitHub
- Render

---

# 🚀 Running the Project Locally

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Start the Flask Server

```bash
python app.py
```

The API will start on:

```
http://127.0.0.1:5000
```

---

# 🔗 API Endpoints

## Home

**GET /**

Returns a confirmation message.

Example Response

```json
{
  "message": "Heart Disease Prediction API is Running!"
}
```

---

## Prediction

**POST /predict**

Example JSON Request

```json
{
    "age":63,
    "sex":1,
    "cp":3,
    "trestbps":145,
    "chol":233,
    "fbs":1,
    "restecg":0,
    "thalach":150,
    "exang":0,
    "oldpeak":2.3,
    "slope":0,
    "ca":0,
    "thal":1
}
```

Example Response

```json
{
    "prediction":"Heart Disease Detected"
}
```

---

# 📈 Model Workflow

```
Heart Dataset
        │
        ▼
Data Preprocessing
        │
        ▼
Train-Test Split
        │
        ▼
Random Forest Model
        │
        ▼
Model Evaluation
        │
        ▼
Save Model (model.pkl)
        │
        ▼
Flask REST API
        │
        ▼
Render Deployment
```

---

# 📌 Future Improvements

- Develop a web-based user interface.
- Add input validation.
- Improve prediction accuracy using hyperparameter tuning.
- Integrate a database for storing patient records.
- Deploy using Docker and CI/CD pipelines.

---

## Conclusion (Task 5)

This project successfully developed and deployed a Heart Disease Prediction system using a Random Forest Classifier. The model demonstrated good performance in predicting the presence of heart disease based on patient health parameters. During deployment, challenges such as configuring the Flask application, managing project files, creating the required dependencies, and deploying the API on Render were encountered and resolved. Testing the API using Postman confirmed that the application was functioning correctly. This project highlights the importance of MLOps in machine learning, as it enables seamless integration of model training, deployment, testing, and maintenance. MLOps ensures that machine learning models are reliable, reproducible, scalable, and easily accessible through APIs, making them suitable for real-world applications.

---

# 📜 License

This project has been developed for academic purposes as part of the Machine Learning Deployment Assignment at VIT Bhopal University.
