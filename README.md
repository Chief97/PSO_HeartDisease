# PSO_HeartDisease

## About Dataset
Key Indicators of Heart Disease
2022 annual CDC survey data of 400k+ adults related to their health status

## What subject does the dataset cover?
According to the CDC, heart disease is a leading cause of death for people of most races in the U.S. (African Americans, American Indians and Alaska Natives, and whites). About half of all Americans (47%) have at least 1 of 3 major risk factors for heart disease: high blood pressure, high cholesterol, and smoking. Other key indicators include diabetes status, obesity (high BMI), not getting enough physical activity, or drinking too much alcohol. Identifying and preventing the factors that have the greatest impact on heart disease is very important in healthcare. In turn, developments in computing allow the application of machine learning methods to detect "patterns" in the data that can predict a patient's condition.

## Where did the data set come from and what treatments has it undergone?
The dataset originally comes from the CDC and is a major part of the Behavioral Risk Factor Surveillance System (BRFSS), which conducts annual telephone surveys to collect data on the health status of U.S. residents. As described by the CDC: "Established in 1984 with 15 states, BRFSS now collects data in all 50 states, the District of Columbia, and three U.S. territories. BRFSS completes more than 400,000 adult interviews each year, making it the largest continuously conducted health survey system in the world. The most recent dataset includes data from 2023. Though the dataset used here was retrieved from Kaggle, an opensource data sharing forum.

## What was done to the data set?
As described above, the dataset retrieved had around 40 variables. In addition to classical EDA, this dataset was used to apply a number of machine learning methods, especially classifier models (logistic regression, SVM, random forest, etc.) and also Particle Swarm Optimization was used to identify most relevant features that gave a bettwe accuracy and Area Under the ROC curve. The variables "HadHeartAttack", "HadAngina" and "HadStroke" were utilized to create the target variable (1 - if respondent had either heart attack, angina or stroke; 0 - if respondent did not have any of these). Note, however, that the classes are unbalanced, so random sampling was applied to the negative class with a ratio calculated such that the entire positive class was retained, to simulate a balanced dataset.
