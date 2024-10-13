Spaceship Titanic: Machine Learning Model for Passenger Survival Prediction
This repository contains a machine learning project that predicts passenger survival for the Spaceship Titanic disaster. 
Using a dataset that includes various features of passengers, this project explores data preprocessing, feature engineering, model building, and evaluation to predict whether passengers were "Transported" to another dimension.

🗂️ Dataset Overview
The dataset used in this project consists of the following features:

PassengerId: Unique identifier for each passenger
HomePlanet: Planet the passenger departed from (Earth, Europa, Mars)
CryoSleep: Indicates if the passenger opted for cryogenic sleep during the voyage
Cabin: Passenger's cabin number (deck/num/side)
Destination: The intended destination for the passenger
Age: Passenger's age
VIP: Whether the passenger paid for special VIP service
RoomService: Amount spent on room service
FoodCourt: Amount spent at the ship’s food court
ShoppingMall: Amount spent at the mall
Spa: Amount spent on the spa
VRDeck: Amount spent on the VR deck
Name: Passenger's name
Transported: Target variable indicating if the passenger was transported to another dimension (0 or 1)

📊 Project Workflow
Data Preprocessing:

Handling missing values in columns like CryoSleep, Age, and HomePlanet.
Feature transformation for variables like Cabin and PassengerId.
Encoding categorical variables such as HomePlanet and Destination.
Feature Engineering:

Creation of new features from the existing ones, such as extracting the deck and side from the Cabin variable.
Aggregating expenses (RoomService, FoodCourt, ShoppingMall, Spa, VRDeck) to create a TotalSpending feature.
Model Building:

Various machine learning models like Random Forest, XGBoost, and Logistic Regression were tested.
Hyperparameter tuning was performed to optimize model performance.
Cross-validation and performance metrics such as accuracy, precision, and recall were used to evaluate models.
Model Evaluation:

The model with the best performance is selected based on metrics like accuracy and AUC-ROC.
Feature importance was analyzed to understand key drivers of passenger survival.

📈 Key Insights
The CryoSleep and VIP status of passengers were significant features for predicting whether they were transported.
Age and total spending also played important roles in survival outcomes.
Feature engineering, especially breaking down the Cabin information, helped improve model accuracy.

🛠️ Tech Stack
Python: For data processing and model building
Pandas, NumPy: For data manipulation
scikit-learn, XGBoost: For building machine learning models
Matplotlib, Seaborn: For visualizing data and insights

📌 Conclusion
This project highlights how machine learning can be applied to predict outcomes from space voyage scenarios. It covers end-to-end machine learning processes including data cleaning, feature engineering, model selection, and evaluation.
