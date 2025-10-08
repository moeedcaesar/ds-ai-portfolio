# 🌾 Crop Recommendation System

📖 **Overview**  
This project is a **web application** that recommends the most suitable crop based on soil, water, climate, and nutrient parameters.  
The app uses a **Random Forest Classifier** trained on a dataset of 57,000 crop samples from [Kaggle Crop Recommendation Dataset](https://www.kaggle.com/datasets/saganachinnathambi/crop-recommendation).

🧠 **Skills Demonstrated**  
- Data cleaning and preprocessing  
- Feature selection for machine learning  
- Encoding categorical variables  
- Training a **Random Forest Classifier**  
- Evaluating model accuracy and feature importance  
- Building a **Streamlit web app** for interactive predictions  
- Visualizing prediction probabilities with Altair  

🧰 **Tools Used**  
Python, Pandas, Scikit-learn, Streamlit, Numpy, Altair  

⚙️ **Methodology**  
1. **Data Preprocessing:**  
   - Selected relevant features: Soil pH, Crop Duration, Temperature, Water, Humidity, and NPK levels.  
   - Encoded the target crop variable into numeric labels for ML.  

2. **Model Training:**  
   - Split the dataset into 80% training and 20% testing.  
   - Trained a Random Forest Classifier.  
   - Achieved **100% accuracy** on the test set.  
   - Identified most important features contributing to crop prediction.  

3. **Web Application (Streamlit):**  
   - Users input soil, water, climate, and nutrient measurements via sliders in 4 tabs.  
   - The app predicts the **best crop** and displays a **top 3 recommended crops** with probabilities.  
   - Visualizes crop recommendation probabilities using an interactive **Altair bar chart**.  

🚀 **Demo**  
- Input sample values to get your crop recommendation:  
  ```python
  input_row = [[7.13, 8.33, 180, 210, 42, 51, 533, 685, 40, 60, 45, 49, 62, 65, 89, 95]]
  model.predict(input_row)  # Output: groundnut
