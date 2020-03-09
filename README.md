# Week 9 Project  
`Pump-it-Up-Data-Mining-the-Water-Table`

# Goal
The goal of this project is to predict which pumps are functional ( or need some repairs), which are not funtional. KNN, Decision Tree and Random Forest are applied in this project. According to accuracy_score and F1_score, Random Forest model is selected as the final model. 

# Data Cleaning  
- In order to obtian the best prediction, I removed some columns which contian missing data more than 20%. Then remove rows which contians missing values.

# Distribution of Target
![distribution_of_target.png](distribution_of_target.png)
 - Because the target size for each class is not balanced, so I applied oversampling method to balance the class size.
# Feature Engineering
- Train Test Split
- Oversampling
- Data Standardization (MinMaxScaler)

# Feature Selection
![matrix.png](matrix.png)
- In this part, I did not remove any features.  

# Models
- KNN         
- Random Forest 
- Decision Tree
# Conclusion
![feature_importance.png](feature_importance.png)
Comparing KNN , Random Forest and Decision Tree models, Random Forest model gave highest accuracy score and F score.  
According to Random Forest model top 5 important features are :
 * 1.'longitude' 
 * 2.'latitude'
 * 3.'quantity'
 * 4.'gps_height'
 * 5.'waterpoint_type'
 
 
 #    
- Source website: https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/data/
- Presentation:
https://docs.google.com/presentation/d/16RuNrFkAatRffgyUuw8Lktg78MtJ3fW1VdPh9muhDoM/edit#slide=id.g52d0ce73e5_0_238
