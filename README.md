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

The heart_disease_cleaned_new.csv containing the dataset used to train ML models, the following are the variables found in it:
'State' (char variable) - Represents the state from which the respondent is from.
'Sex' (char variable) - Represents which sex the respondent belongs t.
'GeneralHealth' (char variable) - Represents the general health of the respondent
'PhysicalHealthDays' (int variable) - Represents the number of physical health days that the respondent has taken.
'MentalHealthDays' (int variable) - Represents the number of mental health days that the respondent has taken. 'LastCheckupTime' (char variable) - (int variable) - Represents the duration since the last time the respondent went for a checkup. 
'PhysicalActivities' (char variable) - Represents the amount of physical activity that the respondent is involved in, on a daily basis. 
'SleepHours' (int variable) - Represents the average number of hours the respondent sleeps on a daily basis. 'RemovedTeeth' (char variable) - Represents if there have been any tooth removed from the respondent during his life time.
'HadAsthma' (char variable) - Represents if the respondent has had any Asthma.
'HadSkinCancer' (char variable) - Represents if the respondent has had any Cancer. 
'HadCOPD' (char variable) - Represents if the respondent has had any Chronic obstructive pulmonary disease (COPD), a disease related to the lung.
'HadDepressiveDisorder' (char variable) - Represents if the respondent has had depression.
'HadKidneyDisease'(char variable) - Represents if the respondent has had kidney disease. 
'HadArthritis' (char variable) - Represents if the respondent has had arthritis.
'HadDiabetes' (char variable) - Represents if the respondent has had diabetes.
'DeafOrHardOfHearing' (char variable) - Represents if the respondent is either/neither deaf or have any hardness in hearing. 
'BlindOrVisionDifficulty' (char variable) - Represents if the respondent is either/neither blind or have any difficulty with vision.
'DifficultyConcentrating' (char variable) - Represents if the respondent has had any difficulty in concentrating.
'DifficultyWalking' (char variable) - Represents if the respondent has had any difficulty walking.
'DifficultyDressingBathing' (char variable) - Represents if the respondent has had any issues handling himself personally.
'DifficultyErrands' - (char variable) - Represents if the respondent has had any problem running errands.
'SmokerStatus' (char variable) - Represents if the respondent is a smoker.
'ECigaretteUsage' (char variable) - Represents if the respondent is a user of Eciggarettes.
'ChestScan' (char variable) - Represents if the respondent has had any chestscan recently.
'RaceEthnicityCategory' (char variable) - Represents to the race and ethnicity of the respondent.
'AgeCategory' (char variable) - Represents the age category group that the respondent belongs to.
'HeightInMeters' (float variable) - Represents the height of the respondent in meters.
'WeightInKilograms' (float variable) - Represents the weight of the respondent in kilograms.
'BMI' (float variable) - Represents the BMI of the respondent.
'AlcoholDrinkers' (char variable) - Represents if the respondent drinks alcohol.
'HIVTesting' (char variable) - Represents if the respondent has HIV/not.
'FluVaxLast12' (char variable) - Represents if the respondent has had Flu vaccine in the past 12 months.
'PneumoVaxEver' (char variable) - Represents if the respondent has had the pneumonia vaccine in his lifetime.
'TetanusLast10Tdap' (char variable) - Represents if the respondent has had the TDAP tetanus vaccine in the past 10 years.
'HighRiskLastYear' (char variable) - Represents if the respondent has taken any high risk the past year.
'CovidPos' (char variable) - Represents if the respondent was COVID Positive. 
'Heart Disease' (binary variable) - The target variable, with 1/0 representing if the respondent has had any heart disease during their lifetime.
