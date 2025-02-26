Machine Learning Engineering Capstone Proposal

# Heart Disease Prediction

## A) Domain Background: Overview

Heart disease is the leading cause of death for people of most racial and ethnic groups in the United States, including African American, American Indian, Alaska Native, Hispanic, and white men. For women from the Pacific Islands and Asian American, American Indian, Alaska Native, and Hispanic women, heart disease is second only to cancer.

- One person dies every 37 seconds just in the United States alone from cardiovascular disease.
- About 647,000 Americans die from heart disease each year—that&#39;s 1 in every 4 deaths.
- Heart disease costs the United States about $219 billion each year from 2014 to 2015. This includes the cost of health care services, medicines, and lost productivity due to death.

## B) Problem Statements

- Complete analysis of Heart Disease UCI dataset both visually and statistically to obtain critical observations which can be used for inference.
- To predict whether a person has a heart disease or not based on the various biological and physical parameters of the body
- To make a model having high accuracy and precision and can predict the results with greater confidence.
- Make these predictions accessible to users and patients anywhere, anytime so that they can get complete picture of their Health

##
## C) Datasets and Inputs

## 1. Collecting Data

The data used for training and testing is the [Heart Disease UCI](https://doi.org/10.24432/C52P4X) downloaded from Kaggle.
This database contains 76 attributes, but all published experiments refer to using a subset of 14 of them. In particular, the Cleveland database is the only one that has been used by ML researchers to this date. The &quot;goal&quot; field refers to the presence of heart disease in the patient.

![image](https://user-images.githubusercontent.com/30470730/72439674-5f9a6a00-37cd-11ea-9366-6ef953b6879e.png)


## 2. Exploratory Data Analysis

It&#39;s a clean, easy to understand set of data. However, the meaning of some of the column headers are not obvious. Here&#39;s what they mean,

- age: The person&#39;s age in years
- sex: The person&#39;s sex (1 = male, 0 = female)
- cp: The chest pain experienced (Value 1: typical angina, Value 2: atypical angina, Value 3: non-anginal pain, Value 4: asymptomatic)
- trestbps: The person&#39;s resting blood pressure (mm Hg on admission to the hospital)
- chol: The person&#39;s cholesterol measurement in mg/dl
- fbs: The person&#39;s fasting blood sugar (\&gt; 120 mg/dl, 1 = true; 0 = false)
- restecg: Resting electrocardiographic measurement (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy by Estes&#39; criteria)
- thalach: The person&#39;s maximum heart rate achieved
- exang: Exercise induced angina (1 = yes; 0 = no)
- ldpeak: ST depression induced by exercise relative to rest (&#39;ST&#39; relates to positions on the ECG plot. See more here)
- slope: the slope of the peak exercise ST segment (Value 1: upsloping, Value 2: flat, Value 3: downsloping)
- ca: The number of major vessels (0-3)
- thal: A blood disorder called thalassemia (3 = normal; 6 = fixed defect; 7 = reversable defect)
- target: Heart disease (0 = no, 1 = yes)

## 3. Data Visualization

Now let&#39;s see various visual representations of the data to understand more about relationship between various features.

![image](https://user-images.githubusercontent.com/30470730/72439765-822c8300-37cd-11ea-8b3e-e0e53fedf0c9.png)

![image](https://user-images.githubusercontent.com/30470730/72439779-89539100-37cd-11ea-80bb-7c721f8e06cb.png)

## 4. Correlation Matrix

The best way to compare relationship between various features is to look at the correlation matrix between those features.

![image](https://user-images.githubusercontent.com/30470730/72439867-bef87a00-37cd-11ea-8613-8144b209d65f.png)

## 5. Data Processing

* We clean data, removing empty rows, and changing columns names to more understandable terms.  
* We then drop the columns which require more complex inputs to make model user-friendly.
* We then proceed to split the data in testing and training sets.

## 6. Inputs

Here our Model is trained to predict whether a person has a heart disease or not based on the following common features as input:

- age
- gender
- chest pain
- blood pressure
- cholesterol level
- max heart rate


## D) Benchmarks

The model will be using a test dataset for benchmarking. The predicted labels will be compared to the original labels to find false positives and false negatives. Number of false positives and false negatives will tell us about the performance of model.

## E) Evaluation Metrics
* Recall:  1.0
* Precision:  1.0
* Accuracy: 0.875

The model will be using various evaluation metrics such as

- Accuracy: which refers to how close a measurement is to the true value and can be calculated using the following formula

![image](https://user-images.githubusercontent.com/30470730/72439883-c586f180-37cd-11ea-94a3-09c09cbd4814.png)


- Precision: which is how consistent results are when measurements are repeated and can be calculated using the following formula

 ![image](https://user-images.githubusercontent.com/30470730/72440009-10a10480-37ce-11ea-8f11-0a3352d0646c.png)

- Recall: which refers to the percentage of total relevant results correctly classified by the model and can be calculated using the formula

 ![image](https://user-images.githubusercontent.com/30470730/72440027-1565b880-37ce-11ea-8bf9-5c5d7a609f85.png)




