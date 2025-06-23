# 🚗 Car Price Prediction  

## 🌟 Overview  
This project focuses on predicting car prices based on various attributes of cars using machine learning techniques. The model is trained on a dataset of car features, including car name, year, selling price, present price, fuel type, seller type, transmission, and kilometers driven.  

---

## 📊 Dataset  
The dataset used in this project is **`car data.csv`**, which includes the following features:  
- 🚘 **Car_Name**: Name of the car.  
- 📅 **Year**: Year of purchase.  
- 💰 **Selling_Price**: The price at which the car is being sold.  
- 🏷️ **Present_Price**: The current ex-showroom price of the car.  
- 🛣️ **Kms_Driven**: The total kilometers driven by the car.  
- ⛽ **Fuel_Type**: The type of fuel the car uses (Petrol/Diesel/CNG).  
- 🧑‍💼 **Seller_Type**: Whether the seller is a dealer or an individual.  
- ⚙️ **Transmission**: Type of transmission (Manual/Automatic).  
- 🏠 **Owner**: The number of previous owners.  

---

## 🔧 Steps Involved  

### 1️⃣ **Data Preprocessing**  
- 📥 Imported the dataset using pandas.  
- 🔍 Explored and cleaned the dataset:  
  - ✅ Checked for missing values and handled them appropriately.  
  - 🔄 Transformed categorical data into numerical form using one-hot encoding.  
  - 🗓️ Extracted the car's age from the `Year` column and dropped unnecessary columns like `Car_Name`.  
- ✂️ Split the dataset into features (X) and target variable (y), where `y` is the `Selling_Price`.  

---

### 2️⃣ **Feature Scaling**  
- ⚖️ Applied scaling to numerical features such as `Present_Price`, `Kms_Driven`, and `Car_Age` to normalize the data and ensure uniformity across features.  

---

### 3️⃣ **Data Splitting**  
- 📤 Split the dataset into training and testing sets with an 80:20 ratio to evaluate model performance effectively.  

---

### 4️⃣ **Model Training**  
The following models were implemented:  
- 🤖 **Linear Regression**: To establish a baseline for predictions.  
- ⚙️ **Ridge Regression**: To mitigate overfitting by applying L2 regularization.  
- 🌲 **Decision Tree Regressor**: For non-linear relationships between features and the target variable.  
- 🌳 **Random Forest Regressor**: To improve accuracy by combining multiple decision trees.  

---

### 5️⃣ **Model Evaluation**  
- 📈 Used metrics such as **R-squared (R²)** and **Mean Absolute Error (MAE)** to evaluate the performance of the models on the test dataset.  
- 📊 Compared the results of each model to determine the best-performing model for the given dataset.  

---

### 6️⃣ **Hyperparameter Tuning**  
- 🔍 Optimized the hyperparameters of the Random Forest Regressor using **GridSearchCV** to achieve the best possible results.  

---

### 7️⃣ **Prediction**  
- 🖥️ Provided a user interface for predicting car prices based on new input values for features like `Present_Price`, `Kms_Driven`, `Fuel_Type`, etc.  

---

## 🏆 Results  
- 🌟 The **Random Forest Regressor** emerged as the best-performing model with high accuracy and low error rates.  

---

## 🛠️ Requirements  
- **Python** (3.7 or above)  
- Libraries:  
  - 🐼 pandas  
  - 🔢 numpy  
  - 📊 matplotlib  
  - 🎨 seaborn  
  - 🧪 sklearn  

Install them using:  
```bash
pip install -r requirements.txt
```
## 🚀 How to Run the Project
1. 🖱️ Clone the repository to your local machine.

2. 📦 Ensure the required libraries are installed using the above command.

3. ▶️ Run the Jupyter Notebook Car Price Prediction.ipynb to explore and execute the project step by step.

## 🌍 Future Scope
✨ Enhancing the model by including more features like car brand popularity.

📚 Incorporating a larger dataset for improved model generalization.

🌐 Deploying the model as a web application for real-time car price predictions.
