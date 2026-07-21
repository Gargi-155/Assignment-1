# Medical Insurance Cost Prediction using Multiple Linear Regression

## Project Information

 **Name:** Gargi 
 **Registration Number:** 23BCE11333  
 **Application Number:** IN26011023 
 **Batch Number:** 2B
 **Email ID:** gargi.23bce11333@vitbhopal.ac.in

---

# Objective

The objective of this project is to develop a **Multiple Linear Regression** model capable of predicting an individual's medical insurance charges based on demographic and health-related attributes. The project demonstrates the complete machine learning workflow, including data preprocessing, model training, evaluation, and performance analysis.

---

# Dataset

**Medical Cost Personal Insurance Dataset**

Source: Kaggle – Medical Cost Personal Insurance Dataset

Dataset Link: https://www.kaggle.com/datasets/mirichoi0218/insurance

The dataset contains information about policyholders, including:

* Age
* Gender
* Body Mass Index (BMI)
* Number of children
* Smoking status
* Residential region
* Medical insurance charges (target variable)

---

# Technologies and Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Kaggle API

---

# Methodology

### 1. Data Collection and Understanding

* Loaded the insurance dataset using Pandas.
* Explored the dataset structure, feature types, and target variable.
* Verified the dimensions and statistical summary of the data.

### 2. Data Preprocessing

* Checked for missing or null values.
* Encoded categorical variables (`sex`, `smoker`, and `region`) using **One-Hot Encoding** with `drop_first=True` to prevent multicollinearity.
* Prepared the dataset for model training.

### 3. Data Splitting

* Divided the dataset into:

  * **80% Training Data**
  * **20% Testing Data**
* Used `train_test_split` from Scikit-learn with a fixed random state for reproducibility.

### 4. Model Development

* Implemented the **Multiple Linear Regression** algorithm using Scikit-learn's `LinearRegression` model.
* Trained the model using all available predictor variables.

### 5. Model Evaluation

The trained model was evaluated using the following performance metrics:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* R² Score (Coefficient of Determination)

An **Actual vs. Predicted** scatter plot was also generated to visualize the model's prediction accuracy.

---

# Results

The trained model achieved the following performance:

* **R² Score:** Approximately **0.78**
* **Mean Absolute Error (MAE):** Evaluated on the test dataset
* **Mean Squared Error (MSE):** Evaluated on the test dataset

### Key Findings

The most influential factors affecting medical insurance charges were:

* Smoking status
* Age
* Body Mass Index (BMI)

The model was able to explain approximately **78% of the variance** in medical insurance costs, indicating good predictive performance for a linear model.

---

# Conclusion

This project demonstrates that **Multiple Linear Regression** can effectively model and predict medical insurance costs using demographic and health-related information. With an R² score of approximately **0.78**, the model successfully captures the overall relationship between the input features and insurance charges.

However, one limitation of linear regression is its inability to capture complex non-linear relationships and feature interactions. For example, the combined impact of high BMI and smoking may not be fully represented by a linear model.

Future improvements could include implementing more advanced machine learning algorithms such as:

* Random Forest Regressor
* Gradient Boosting Regressor
* XGBoost Regressor

These models can better capture non-linear relationships and are likely to provide higher predictive accuracy.

---

# Future Scope

* Perform feature engineering to improve model performance.
* Apply hyperparameter tuning to optimize predictive accuracy.
* Compare Multiple Linear Regression with ensemble learning models.
* Deploy the trained model as a web application using Flask or Streamlit for real-time insurance cost prediction.
