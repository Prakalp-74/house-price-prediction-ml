# 🏠 House Price Prediction using Machine Learning

## 📌 Project Overview

This project builds a **House Price Prediction model** using Linear Regression.
The goal is to predict the price of a house based on features like area, number of bedrooms, bathrooms, parking, and other housing attributes.

This project demonstrates a complete **Machine Learning workflow**, including data preprocessing, model training, evaluation, and visualization.

---

## ⚙️ Technologies Used

* Python
* pandas
* NumPy
* scikit-learn
* Matplotlib

---

## 📂 Dataset

The dataset contains housing information with the following features:

* area
* bedrooms
* bathrooms
* stories
* mainroad
* guestroom
* basement
* hotwaterheating
* airconditioning
* parking
* prefarea
* furnishingstatus
* price (target variable)

---

## 🔎 Project Workflow

### 1️⃣ Data Cleaning

* Loaded dataset using pandas
* Checked for missing values
* Verified data types

### 2️⃣ Feature Engineering

* Converted categorical variables using one-hot encoding (`get_dummies`)
* Prepared feature matrix **X** and target variable **y**

### 3️⃣ Train-Test Split

The dataset was split into:

* **80% Training data**
* **20% Testing data**

Using `train_test_split()`.

---

### 4️⃣ Model Training

Used **Linear Regression** to train the model.

```
model = LinearRegression()
model.fit(X_train, y_train)
```

---

### 5️⃣ Predictions

The trained model predicts house prices on the test dataset.

```
predictions = model.predict(X_test)
```

---

### 6️⃣ Model Evaluation

**R² Score**

Measures how well the model explains variance in the data.

```
R² Score ≈ 0.65
```

**Mean Squared Error (MSE)**

Measures the average squared difference between predicted and actual values.

```
MSE ≈ 1.75 × 10¹²
```

---

### 7️⃣ Visualization

A scatter plot was used to compare **Actual vs Predicted house prices**.

```
plt.scatter(y_test, predictions)
plt.xlabel("Actual Price")
plt.ylabel("Predicted Price")
plt.title("Actual vs Predicted House Prices")
plt.show()
```

This helps visually evaluate how well the model predictions match the actual prices.

---

## 📊 Results

* Model: Linear Regression
* R² Score: **0.65**
* Model successfully predicts house prices based on housing features.

---

## 📁 Project Structure

```
house_prediction_ml
│
├── Housing.csv
├── practice_house_prediction.ipynb
├── house_price_model.pkl
└── README.md
```

---

## 🚀 Future Improvements

* Try advanced models like Random Forest or Gradient Boosting
* Perform feature scaling
* Hyperparameter tuning
* Improve model accuracy

---

## 👨‍💻 Author

**Prakalp**
AI & Data Science Student

This project is part of my **Machine Learning learning journey**.
