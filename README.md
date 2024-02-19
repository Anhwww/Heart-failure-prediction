# Heart-failure-prediction
This is a project mainly I tried to learn techniques used in Exploratory Data Analysis (EDA).

There are 5 models used here: 
1.	Logistic Regression	
2.	Support Vector Classifier	
3.	Decision Tree Classifier	
4.	Random Forest Classifier	
5.	K-Nearest Neighbors Classfier	

Aim: To classify / predict whether a patient is diagnosed with heart failure depending on multiple attributes.

## Data Attributes:

* Age : age of the patient [years]
* Sex : sex of the patient [M: Male, F: Female]
* ChestPainType : chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
* RestingBP : resting blood pressure [mm Hg]
* Cholesterol : serum cholesterol [mm/dl]
* FastingBS : fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
* RestingECG : resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
* MaxHR : maximum heart rate achieved [Numeric value between 60 and 202]
* ExerciseAngina : exercise-induced angina [Y: Yes, N: No]
* Oldpeak : oldpeak = ST [Numeric value measured in depression]
* ST_Slope : the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
* HeartDisease : output class [1: heart disease, 0: Normal]

## Feature preprocessing
* Calculate the mean values of all the features for cases of heart diseases and non-heart diseases.
* Visualize the distribution of all features
* Check the correlation only with respect to HeartDisease.

## Conclusion for EDA part:

1. Order / Values of features for positive cases of heart disease :

a. Categorical Features (Order) :
* Sex : Male > Female
* ChestPainType : ASY > NAP > ATA > TA
* FastingBS : ( FBS < 120 mg/dl ) > ( FBS > 120 mg/dl)
* RestingECG : Normal > ST > LVH
* ExerciseAngina : Angina > No Angina
* ST_Slope : Flat > Up > Down

b. Numerical Features (Range) :
* Age : 50+
* RestingBP : 95 - 170
* Cholesterol : 160 - 340
* MaxHR : 70 - 180
* Oldpeak : 0 - 4

2. Distribution of numerical and categorical features
* Cholesterol and MaxHR has a bidmodal data distribution which means there is a separation between the two groups within the dataset but in feature MaxHR these 2 group are not clearly seperated.
* Oldpeak's data distribution is rightly skewed.
* All the categorical features closely followed the normal distribution.

Reference: https://www.kaggle.com/

