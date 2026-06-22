# 📊 Machine Learning Model Training and Evaluation Basics

## 📌 Project Overview

This project demonstrates the fundamental steps involved in building a Machine Learning regression model using Scikit-Learn.
The notebook covers data splitting, model training, prediction generation, and error analysis using Linear Regression.
It is designed as a beginner-friendly introduction to supervised learning workflows.

---

## 🎯 Objective

To understand how machine learning models are trained and evaluated using training and testing datasets.

---

## 🛠️ Technologies Used

- Python
- Pandas
- Scikit-Learn

---

## 📂 Dataset

### Feature
- Years of Experience

### Target
- Salary

---

## 🔍 Workflow

### 1. Data Loading

Imported the salary dataset using Pandas.

```python
df = pd.read_csv('Salary_Data.csv')
```

### 2. Feature and Target Selection

```python
x = df[['YearsExperience']]
y = df['Salary']
```

### 3. Train-Test Split

```python
Xtrain, Xtest, Ytrain, Ytest = train_test_split(
    x,
    y,
    train_size=0.8,
    random_state=42
)
```

Training Data: 80%

Testing Data: 20%

---

### 4. Model Training

```python
model = LinearRegression()
model.fit(Xtrain, Ytrain)
```

The model learns patterns from the training dataset.

---

### 5. Prediction

```python
Ypred = model.predict(Xtrain)
```

The trained model generates salary predictions based on years of experience.

---

### 6. Error Analysis

```python
Error = Ytrain - Ypred
```

The prediction error represents the difference between actual and predicted values.

---

## 📈 Concepts Covered

- Supervised Learning
- Linear Regression
- Train-Test Split
- Model Training
- Model Prediction
- Error Analysis
- Machine Learning Workflow

---

## 💡 Skills Demonstrated

- Data Preparation
- Feature Selection
- Model Training
- Prediction Generation
- Regression Fundamentals
- Scikit-Learn Implementation

---

## 📁 Project Structure

```
ML-Training-Basics/
│
├── ml6data.ipynb
├── Salary_Data.csv
└── README.md
```

---

## 🚀 Future Improvements

- Add R² Score Evaluation
- Add MAE and RMSE Metrics
- Visualize Regression Line
- Evaluate on Test Data
- Compare Multiple Regression Models

---

## 👨‍💻 Author

Udaya Kumar B Totta

Computer Science Engineering Student  
Machine Learning | Data Science | Python