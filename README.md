# Week 9 Project  
`Pump-it-Up-Data-Mining-the-Water-Table`

# Goal
The goal of this project is to predict which pumps are functional or functional but need some repair, which are not functional. KNN, Decision Tree and Random Forest are applied in this project. According to accuracy_score and F1_score, Random Forest model is selected as the final model. 

## Target: 
- not functional :0
- functional :1
- functional but need to repair :2

## Predictors:
![feature_table.png](feature_table.png)
           
# Data Cleaning
- [Enders ( 2003 ) stated that a missing rate of 15% to 20% was common in educational and psychological studies.](https://psycnet.apa.org/record/2003-09632-006) In order to obtain the best prediction, some columns which contian missing data more than 20% were removed.  There are 29 predictors(columns), the rows which contians more than 10 were removed. 

# Distribution of Target
-![distribution_of_target.png](distribution_of_target.png)
- Due to the sizes for each class are not balanced, Oversampling method was applied to balance the class size.
 
# Feature Engineering
- Train Test Split
- Oversampling
- Data Standardization (MinMaxScaler)
- Feature Selection:  According to the Correlation Maxtrix below, there are no siginificant corrlation between two predictiors, however only one predictor - waterpoint_type_group got removed. Besides waterpoint_type contians similar information and can also explain waterpoint_type_group.  
  
![matrix.png](matrix.png)


# Models
- KNN         
- Random Forest 
- Decision Tree

# Conclusion
- After model evaluation, Random Forest model is the best model with highest accuarcy score and f1 socre. 
 ![prediction_VS_actual.png](prediction_VS_actual.png)
 ![confusion_matrix.png](confusion_matrix.png)
  
- Comparing KNN , Random Forest and Decision Tree models, Random Forest model gave highest accuracy score and F score.  
According to Random Forest model top 5 important features are :
 * 1.'longitude' 
 * 2.'quantity'
 * 3.'latitude'
 * 4.'gps_height'
 * 5.'ward'
 
![feature_importance.png](feature_importance.png)

 
 #    
- Source website: https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/data/
- Presentation:
https://docs.google.com/presentation/d/16RuNrFkAatRffgyUuw8Lktg78MtJ3fW1VdPh9muhDoM/edit#slide=id.g52d0ce73e5_0_238
- Dashboard:
https://public.tableau.com/profile/hua.shi#!/vizhome/WaterPumpsProject/water_pump_classification_project
