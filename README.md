# 📊 Profit Prediction Using Machine Learning (Regression)

## 📌 Project Overview
This project focuses on predicting **profit** for retail orders using **machine learning regression models**.  
The dataset contains order, product, customer, and sales-related information.  
The goal is to analyze historical data, perform exploratory data analysis (EDA), preprocess the data, and build predictive models to accurately estimate profit.

---

## 🎯 Objective
To build a regression model that predicts **profit** based on order details, product category, region, pricing, discount, and sales information.

---

## 🗂️ Dataset Description
The dataset contains the following features:

- **Order Details**: order_date, ship_mode, segment  
- **Geographical Data**: country, city, state, region, postal_code  
- **Product Information**: category, sub_category, product_id  
- **Sales Metrics**: quantity, discount, sale_price, revenue, profit  
- **Time Features**: year, month  

Target Variable:
- **profit**

---

## 🔍 Exploratory Data Analysis (EDA)
The following analyses were performed:

- Checked for missing values and handled them appropriately
- Analyzed distributions of numerical variables
- Identified outliers using boxplots
- Studied profit and revenue trends across categories and regions
- Performed correlation analysis to understand relationships between numerical features
- Analyzed seasonal trends using year and month

---

## ⚙️ Data Preprocessing
The preprocessing steps include:

- Dropping unnecessary columns (`order_id`, `order_date`, `product_id`)
- Splitting data into features (X) and target (y)
- Separating numerical and categorical features
- Encoding categorical variables using **OneHotEncoder**
- Scaling numerical features using **StandardScaler**
- Combining encoded and scaled features into a final dataset
- Splitting the data into training and testing sets (80/20)

---

## 🤖 Machine Learning Models
The following regression models were trained and evaluated:

1. **Linear Regression** (Baseline Model)
2. **Decision Tree Regressor**
3. **Random Forest Regressor**
4. **XGBoost Regressor**

---

## 📈 Model Evaluation Metrics
Models were evaluated using:

- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**
- **R² Score**

A comparison table was created to identify the best-performing model.

---

## 🔧 Hyperparameter Tuning
- **GridSearchCV** was applied to tune hyperparameters for the Random Forest and XGBoost models
- Cross-validation was used to ensure model stability and reduce overfitting
- The best estimator was selected based on the highest R² score

---

## 🏆 Best Model
The **tuned Random Forest / XGBoost Regressor** achieved the best performance with improved accuracy and generalization on unseen data.

---

## 🔮 Prediction
The final model was used to predict profit on new/unseen order data.

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost


---

## 🚀 How to Run the Project
1. Clone the repository  
   git clone https://github.com/TheAImentor/Retail-sales-Analysis.git
   
2. Install dependencies
    pip install -r requirements.txt

3. Run the Jupyter Notebook
   jupyter notebook


📌 Future Improvements

1. Feature selection and dimensionality reduction
2. Advanced hyperparameter tuning
3. Model deployment using Streamlit or Flask
4. Building a dashboard for business insights
