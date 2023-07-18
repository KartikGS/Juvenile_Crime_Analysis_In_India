# Juvenile Crime Analysis

Using data exploration, data analysis and machine learning.

## Objective

Main objective of the analysis is prediction and interpretation of juvenile crime in India and deciding efﬁcient allocation of resources in the right areas to minimise the crime rate.

## Dataset

### Juvenile Crime in India 
Dataset we have considered:[Drive](https://drive.google.com/drive/folders/1zQ7h-ce14K4Lxu4ToFuyUxq3OFvJWPTl?usp=sharing)

### Crime in India (Kaggle)
Following link contains processed data of various crime in separate csv ﬁle. From which we have considered csv which contains information about juvenile crime:[Kaggle](https://www.kaggle.com/datasets/rajanand/crime-in-india)

### Crime in India (NCRB)
Following link contains the original unprocessed data of various crime in separate csv ﬁle:[NCRB](https://ncrb.gov.in/en/crime-in-india)

## Metadata
The dataset contains different sub datasets, each of these sub datasets holds the aggregate value of crime recorded from 2001 to 2010 and are split on various categories. On sub-dataset divided based on:
* Age-group and type of crime
* Background
* Recidivism
The kaggle dataset was preprocessed, various combinations of datasets was used to train the model and address various issues.

## Problem Statements And Results

### Given state, crime(mapping required, not considered for now), age, gender, predicting the possibility of SLL(Naive bias using above data + ARIMA to predict current year using previous year data)

SLL by parima<br>

![Alt text](images/sll.png?raw=true "SLL by parima")

##### Naive Bayes Result
Boys<br>

![Alt text](images/boys.png?raw=true "Boys")<br>

Girls<br>

![Alt text](images/girls.png?raw=true "Girls")

### Feature Importance(Using Linear Regression and Random Forest)

Relation between punishment and recidivism (Linear Regression)<br>

![Alt text](images/finr.png?raw=true "")
![Alt text](images/fior.png?raw=true "")<br>

Relation between punishment and recidivism (Random Forest)<br>

![Alt text](images/finrf.png?raw=true "")
![Alt text](images/fiorf.png?raw=true "")<br>

Background of juveniles committing crime<br>

![Alt text](images/fib.png?raw=true "")
![Alt text](images/fibf.png?raw=true "")

### Which State requires better rehabilitation facilities.(Done using clustering)

![Alt text](images/rn.png?raw=true "")
![Alt text](images/ro.png?raw=true "")

### Given State, who to be on a look out for?(Arima+Naive bias, 3 class classiﬁcation)

Recidivism by parima<br>
![Alt text](images/lo.png?raw=true "Recidivism by parima")<br>

Naive Bayes Result<br>
![Alt text](images/fl.png?raw=true "Naive Bayes Result")

## Future Scope
The next step is to streamline the data analysis process by improving the collection method of data or aggregation of various data. Better interpretations can be made with more abstract data. A lot of key information is lost in the current format of data aggregation.