# Maternal Health Risk Prediction using Machine Learning

## Dataset
- MH.csv
- link: https://github.com/VincentAbas/Maternal-Health-Risk-Prediction/blob/4d5b2ebc53d6c0cfbced9ccb8299a33320bd5ff5/MH.csv

## Data Info
- Age = User/Patient's Age
- SystolicBP = Systolic Blood Pressure
- DiastolicBP = Diastolic Blood Pressure
- BS = Blood Sugar
- BodyTemp = Body Temperature
- HeartRate = Heart Rate
- Risk = Risk Level (Low Risk, Med Risk, High Risk)

## Key Highlights
- Data preprocessing with Z-score outlier removal
- Class balancing with SMOTE
- Random Forest base model vs GridSearchCV model
- Performance evaluation with Classification Report and Confusion Matrix
  
## Tools used
- Python, Pandas, NumPy, Scikit-learn, Imbalanced-learn, Matplotlib, Seaborn.

# Model Building Process

### **Data Preprocessing**  
- Removed outliers using **Z-score**  
- Standardized numerical features  

### **Handling Class Imbalance**  
- Applied **SMOTE (Synthetic Minority Over-sampling Technique)** to prevent biased predictions  

### **Model Selection & Training**  
- **Base Model:** Random Forest  
- **GridsearchCV Model:**  

### **Performance Evaluation**  
- Compared **before & after GridSearchCV** using:  
- **Confusion Matrix Visualization**  
- **Classification Report (Precision, Recall, F1-score)**
  
## Results and Insights
![Base vs GridSearchCV Random Forest](https://github.com/user-attachments/assets/8f5abf3f-87cf-41ea-80d3-73e18310008a)
- **GridsearchCV** **did not** improve the model, however the set parameters for the GridSearchCV was limited because of the lack of time and resources to find the right parameters. GridsearchCV usually improves the model when the hyperparameters are optimized correctly so it requires more fine tuning but it is time consuming.

![Confusion Matrix](https://github.com/user-attachments/assets/e291f9db-2f8b-400b-8c2a-37213a0a93bb)
- Confusion Matrix showed fewer false negatives as seen in the image there are only 2 High Risk that were predicted as Low Risk and 3 High Risk predicted as Medium Risk therefore making the model safer for real-world use.


