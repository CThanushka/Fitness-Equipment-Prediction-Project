# 🏋️‍♂️ Fitness Program Goal Prediction

## 📘 1. Introduction and Problem Statement

The **Fitness Program Goal Prediction** project aims to create a machine learning model capable of predicting an individual’s **Equipment type (“Full Gym” / “At Home”)** suitable for their preferences and fitness level.
This project applies **supervised learning** techniques to analyze data patterns and automate workout recommendations.

### 1.1 Problem Statement

Selecting appropriate workout programs or equipment can be difficult for individuals without professional guidance.
This system predicts the most suitable workout goal or equipment, reducing manual decision-making and improving user experience in digital fitness applications.

### 1.2 Objectives

* Develop a machine learning model capable of accurately predicting workout goals.
* Compare multiple algorithms to select the best-performing model.
* Optimize model performance using hyperparameter tuning.
* Analyze ethical and bias aspects in model development.

---

## 📊 2. Dataset Description

The dataset used for this project is sourced from **Kaggle** and contains **2,500+ workout entries**.
It includes **9 independent features** such as *Title, Description, Goal,* and *Level*, and one target label representing the equipment or goal category.

**Challenges:** inconsistent data formats, missing values, and class imbalance.

---

## 🧹 3. Data Preprocessing and Exploratory Data Analysis (EDA)

### 3.1 Preprocessing Steps

* Removed duplicates and irrelevant entries
* Dropped missing values
* Cleaned text (removed punctuation, emojis, stopwords)
* Converted string-based lists into usable formats
* Treated outliers in numerical columns
* Standardized feature scaling using `StandardScaler`
* Encoded categorical variables using `LabelEncoder`
* Split data into **training** and **testing** sets

These steps ensured data consistency and model readiness. Scaling and encoding improved convergence and prevented feature dominance.

### 3.2 Exploratory Data Analysis (EDA)

EDA explored:

* Class distribution and imbalance
* Correlation between features
* Outlier detection
  Visualizations (bar plots, histograms) provided insights into data behavior.

---

## 🧠 4. Model Design and Implementation

### 4.1 Models Developed

* Logistic Regression
* Random Forest
* XGBoost
* Support Vector Machine (SVM)

### 4.2 Implementation Environment

Developed in **Python** using **Jupyter Notebook**.
Libraries: `scikit-learn`, `XGBoost`, `NumPy`, `Pandas`, `Matplotlib`.

### 4.3 Model Training and Hyperparameter Tuning

* Used `GridSearchCV` with **5-fold cross-validation**
* Tuned parameters: regularization strength (C), learning rate, max depth, etc.
* Balanced bias–variance tradeoff to achieve optimal performance

---

## 📈 5. Evaluation and Comparison

| Model               | Accuracy   | Precision | Recall    |
| :------------------ | :--------- | :-------- | :-------- |
| Logistic Regression | 0.6245     | 0.776     | 0.659     |
| Random Forest       | 0.6883     | 0.761     | 0.775     |
| SVM                 | 0.6316     | 0.829     | 0.618     |
| **XGBoost**         | **0.7045** | **0.782** | **0.786** |

✅ **XGBoost** achieved the highest accuracy (0.7045) and was selected as the **final model** for deployment.
It provided strong generalization and balanced precision–recall performance.

---

## ⚖️ 6. Ethical Considerations and Bias Mitigation

* The dataset showed slight imbalance across fitness goals.
* Applied **cross-validation** and **resampling** to reduce bias.
* Ethical evaluation ensured fair predictions and prevented misuse.
* The system acts as a **recommendation tool**, not a diagnostic model.

---

## 💡 7. Reflections and Lessons Learned

* Data preprocessing and evaluation are critical for robust results.
* Overfitting in Logistic Regression and SVM required regularization.
* Learned practical ML workflow: from cleaning to tuning to ethical assessment.
* Demonstrated the real-world potential of AI in fitness personalization.

---

## 📚 8. References

1. [Kaggle – Workout Preferences and Fitness Goals Dataset](https://www.kaggle.com/datasets/fitness-and-workout-dataset)
2. [Scikit-learn Documentation](https://scikit-learn.org/)
3. [XGBoost Documentation](https://xgboost.readthedocs.io/)
4. [Python Documentation](https://docs.python.org/3/)

---

## 👨‍💻 Author

**Chamuditha Thanushka**
📩 Reach out for collaborations or suggestions!
