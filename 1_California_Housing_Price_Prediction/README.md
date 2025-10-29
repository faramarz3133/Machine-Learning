# 🏠 California Housing Price Prediction

This project focuses on predicting **median house values** in California districts using the **California Housing dataset**.  
The dataset includes information such as median income, average number of rooms, population, and location.  
The goal is to build and compare regression models that can accurately predict house prices.

---

## 🎯 Objective
To develop a machine learning model that can predict the **median house price** (`MedHouseVal`) based on various features from the dataset.

---

## 📊 Dataset
- **Source:** `fetch_california_housing()` from `scikit-learn`
- **Number of Samples:** 20,640
- **Number of Features:** 8 (e.g., MedInc, AveRooms, HouseAge, etc.)
- **Target Variable:** Median House Value

---

## ⚙️ Project Steps

1. **Data Loading & Exploration**
   - Load dataset using `fetch_california_housing`  
   - Display basic statistics and data types  
   - Check for missing values  

2. **Exploratory Data Analysis (EDA)**
   - Visualize feature distributions using histograms  
   - Correlation heatmap between variables  
   - Scatter plots for income vs. house value  

3. **Data Preprocessing**
   - Split data into training and testing sets  
   - Apply feature scaling using `StandardScaler`

4. **Model Building**
   - Train different regression models:
     - Linear Regression  
     - Decision Tree Regressor  
     - Random Forest Regressor  
   - Evaluate using **R²**, **MAE**, and **RMSE**

5. **Model Optimization**
   - Use `GridSearchCV` to tune hyperparameters of Random Forest  
   - Compare results before and after tuning

6. **Results Visualization**
   - Plot predicted vs. actual values  
   - Display feature importances from the best model

---

## 🧠 Key Learnings
- How to handle and analyze real-world housing data  
- Regression modeling using multiple algorithms  
- Hyperparameter tuning using `GridSearchCV`  
- Visualization of model performance and feature importance  



## Author
- Faramarz Aghajani
- faramarzaghajani217@gmail.com
- https://github.com/faramarz3133