# Drug risk and personality traits

The authors: [Mirko Knoche](https://github.com/CrazyBigFoot) & Nina Notman

This project is still **in progress**.

![alt text](https://cdn.pixabay.com/photo/2018/09/13/02/17/pills-3673645_1280.jpg)

## Overview 

This project is based on the [drug use (quantified) data set] (https://archive.ics.uci.edu/ml/datasets/Drug+consumption+%28quantified%29) by Elaine Fehrman. Here, we investigate the relationship between personality traits and drug use risk. The database was collected by Elaine Fehrman between March 2011 and March 2012. The dataset contains 1885 participants. Participants were questioned concerning their use of 18 legal and illegal drugs (alcohol, amphetamines, amyl nitrite, benzodiazepines, cannabis, chocolate, cocaine, caffeine, crack, ecstasy, heroin, ketamine, legal highs, LSD, methadone, magic mushrooms, nicotine and volatile substance abuse). In order to assess personality traits of the sample, the Revised NEO Five-Factor Inventory (NEO-FFI-R) and Barratt Impulsiveness Scale (BIS-11) questionnaire was employed. 

We first coded ormalized demographic data into more understandable numerical categories. For deepder analysis, an additional features was developed: consumption of highly addictive drugs. A participant is categorized as consuming highly addictive drugs if he/she consumes any of the following drugs: heroin, ecstasy, LSD, Cocaine or Meth. Following, we applied ML to predict (1) Cannabis consumption and (2) consumption of highly addictive drugs. 

Business Case: 

Early prediction of drug usage based on personality traits could be interesting for preventive organizations and medical employees. 

The project was part of a data science boot camp and was intended to cover all stages of the data science cycle:

## Life cycle of data science

- 1 Business understanding
- 2 Data acquisition
- 3 Data cleansing
- 4 Data Exploration
- 5 Feature Engineering
- 6 Predictive modeling
- 7 Data visualization

## Used Python modules:
Pandas / NumPy / Matplotlib / Seaborn / sklearn
 
## ML models used
The models were applied and compared for f1 and accuracy values

- K-nearest neighbors 
- Logistic Regression 
- XGBClassifier
- RandomForestClassifier
- Support Vector Machine
 
## Conclusions
- A reliable prediction of cannabis or highly addictive drug consumption is  possible, including demographic data (age, gender, education status),  NEO-FFI-R scores (neuroticism, extraversion, openness, agreeableness, conscientiousness) and BIS-11 scores (impulsive, sensation-seeking)
- We found that age, sensation-seeking, education and openness (in respective order) are the very important personality traits when predicting cannabis consumption. 
- Similarly, openness, agreeableness, neuroticism, extraversion and sensation-seeking (in respective order) are the most important personality traits when predicting highly addictive drug consumption.

## Future work
**Collect more data to generalize model across nations**
- Collect  non-user data 
- Collect data of non-white ethnicity 

**Collect more data to predict clinical information**
- Collect data on the amount of drug doses
- Collect data on clinical diagnoses and adiction history

**Model-related effects:**
- Feature engineering regarding different groups of drugs 
- Try unsupervised machine learning models
- Apply regression models to continuous data

