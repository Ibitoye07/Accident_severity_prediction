# Accident Severity Prediction
Road traffic accidents are a major public safety concern worldwide, causing significant loss of life, injuries, and economic damage each year. Understanding and predicting the severity of these accidents can help authorities and policymakers deploy preventive measures, optimize emergency response, and improve road safety strategies.

This project applies machine learning techniques to analyze traffic accident data and predict accident severity based on factors such as road conditions, weather, time of day, and vehicle involvement. The goal is to develop a predictive model that can assist in proactive safety measures, enhance situational awareness, and ultimately reduce the human and economic toll of road accidents.

# 📋 Project Overview
The project involves:

🧹 Data Preprocessing
🔍 Exploratory Data Analysis
⚙️ Feature Engineering
🧠 Model Training and Evaluation


# Exploratory Data Analysis
From the boxplot, it is evident that outliers exist in each column. The following will examine the outliers to see if they are useful or not:

![image alt](https://github.com/Ibitoye07/Accident_severity_prediction/blob/main/boxplot.png?raw=true)

**Number of vehicles involved**:

The slight injury category have outliers in which 7 cars are involved. This indicates that an accident involving 7 vehicles resulted in slight injuries. At first, I assumed an accident involving this number of vehicles should result in serious or even fatal injuries. While this assumption is valid, certain situations exempt this. As you are reading this, i want you to imagine a scenario of a traffic pile-up, which we all must have seen on some occasions. In this scenario, cars often move at a slow speed in congested lanes. it may take just one vehicle to hit another, setting off a chain reaction (Newton's 3rd law of motion) crash at a slow speed, which might result in minor cuts known as Slight Injuries in this case. This event is quite rare but realistic, and it also shows that all outliers observed represent true cases and should be retained.

**Number of casualties**:

The outliers identified here are valid rather than errors. For example, the Slight injury category includes outliers where up to 8 casualties were recorded, while serious injury shows outliers with up to 6 casualties. These are valid, as it is possible for an accident involving multiple people to result in all or some of them sustaining either slight or serious injuries. Therefore, all outliers should not be discarded, as they represent true events within the context of road traffic accidents.

# Models
Tree based models:
- Decision Tree
- Random Forest
- Xgboost
Neural Network

# Results
Finetuned XGBoost is the best performing tree model
- Recall - 85%
- F1 score - 81%  

Neural Network
- Recall - 80%
- F1 score - 78%

**Top Features**: Number of casualties, Number of vehicles involved and Age band of driver

# Future Scope
- Deploy a streamlit app

# 🙌 Acknowledgments
Special thanks to:

📊 Providers of the dataset used for training the models


