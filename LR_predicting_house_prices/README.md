# 🏠 House Price Prediction using Linear Regression

📖 **Overview**  
This project predicts house prices using **Multiple Linear Regression** based on property features such as area, number of bedrooms, bathrooms, stories, and amenities.  
The goal is to build a predictive model for real estate price estimation.

🧠 **Skills Demonstrated**  
- Data cleaning and preprocessing  
- Encoding categorical features (binary mapping and one-hot encoding)  
- Feature selection and splitting data into training and testing sets  
- Building a Linear Regression model  
- Model evaluation using scatter plots for actual vs predicted values  

🧰 **Tools Used**  
Python, Pandas, Scikit-learn, Matplotlib, Seaborn  

⚙️ **Methodology**  
1. **Data Preprocessing:**  
   - Converted binary categorical features (`yes`/`no`) into numeric values.  
   - Applied **One-Hot Encoding** to the `furnishingstatus` feature.  
2. **Modeling:**  
   - Split the dataset into training (80%) and testing (20%) sets.  
   - Trained a **Linear Regression** model on the training set.  
3. **Evaluation:**  
   - Predicted house prices on the test set.  
   - Visualized model performance using a scatter plot comparing **actual vs predicted prices**.  
   - A 45° reference line was plotted to indicate perfect predictions.  

🚀 **Results**  
- The scatter plot shows that the predicted prices closely follow the actual prices, indicating a good model fit.  
- This model can be used for preliminary price estimation and analysis in the housing market.  

📊 **Visualization**  
- Scatter plot of **Actual Prices vs Predicted Prices** with a 45° reference line.  
- Helps in visually assessing the accuracy of the regression model.  

📂 **Notebook**  
See [`LR_housing.csv.ipynb`](./LR_housing.csv.ipynb)
