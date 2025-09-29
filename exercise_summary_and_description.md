# Smartphone Movement Classification with Machine Learning

## 🔍 Exercise Pitch

In this 3-4 hour exercise, you will explore how sensor data from a smartphone can be used to classify human movements like walking, running, and jumping using different machine learning models.

You will:
- Collect your own movement data with your phone **or** use a provided dataset
- Use a pre-prepared Jupyter Notebook to:
  - Clean and preprocess the data
  - Experiment with KNN, Softmax Regression, and a Recurrent Neural Network
  - Evaluate and compare performance

### 🎯 Target Audience
- Experienced engineers new to machine learning
- Python knowledge not required, but helpful

---

## 📋 Exercise Description

### Step 1: Collect Your Own Sensor Data (Optional)
- Download **Sensor Record** (Android) or similar app
- Record at least 10 seconds of:
  - Walking
  - Running
  - Jumping
  - Push-ups
- Export as `.csv` (accelerometer & gyroscope recommended)

**Or** skip this step and use the `mock_sensor_data.csv` provided.

---

### Step 2: Open the Notebook
- Launch the Jupyter Notebook: `sensor_classification_exercise.ipynb`
- No coding required unless you want to customize further
- Code is fully commented and outputs are interactive

---

### Step 3: Explore Models
- Visualize sensor signals
- Understand the impact of:
  - Raw vs. engineered features (e.g. standard deviation)
  - Scaling
  - Classifier choice
- Try:
  - K-Nearest Neighbors (KNN)
  - Softmax Regression
  - Recurrent Neural Network (LSTM)

---

### 📌 Learning Objectives
- Understand the value of **good data** and simple pre-processing
- Compare pros/cons of different ML models
- Appreciate the importance of feature engineering over brute-force tuning
