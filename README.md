# **BREAST CANCER PREDICTION**

> _Table of Contents_\
> [Libraries](#1-libraries)\
> [Data Source](#2-data-source)\
> [Project Workflow](#3-project-workflow)\
> [Training](#4-training)\
> [Test](#5-test)\
> [Confusion Matrix](#6-confusion-matrix)\
> [Conclusion](#7-conclusion)

![Breast Cancer Predication](assets/cover.png)


## 1. Libraries
1. numpy
2. pandas
3. matplotlib.pyplot
4. seaborn as sns
5. sklearn

## 2. Data source

> This breast cancer databases was obtained from the University of Wisconsin Hospitals, Madison from Dr. William H. Wolberg
>
> O. L. Mangasarian and W. H. Wolberg: "Cancer diagnosis via linear  programming", SIAM News, Volume 23, Number 5, September 1990, pp 1 & 18.
>
> It can be downloaded from  [UCI Machine Learning Repository][1]

## 3. Project Workflow
The workflow for this project is listed below:
1. Pre-processing 
2. Exploratory Data Analysis (EDA)
3. Data Visulization
4. Feature Seletion
5. Train-Test
6. Confusion Matrix
7. Conclusion

## 4. Training
We tried **Four** Machine Learning Models and evaluated their performance with our Dataset. 

### 4.1. Training Results     
The models are listed with their training accuracy below:
> 1. **Decision Tree**: Mean accuracy = 0.**954974** & Std accuracy is **0.020103**
> 2. **Support Vector Machine**: Mean accuracy = **0.971386** & Std accuracy = **0.013512**
> 3. **Gaussian Naive Bayes**: Mean accuracy = **0.963223** & Std accuracy = **0.025463**
> 4. **KNN', K-Nearest Neighbors:** Mean accuracy = **0.969345** & Std accuracy = **0.016428**

## 5. Test
Training shows that the Support Vector Machine model has the highest training accuracy. So we further tested our test dataset with **SVC** and the Test Accuracy was **0.9714285714285714** (97.14%)


### 5.1. Random Testing

> We provided a list of numbers as an input for nine features and it accurately predicted the class for breast cancer.

![Example Prediction for Benign](assets/benignPred.PNG)

![Example Prediction for Malignant](assets/malignantPred.PNG)

## 6. Confusion Matrix
Confusion Matrix from our Validation is:

![Confusion Matrix!](assets/cm.PNG)

## 7. Conclusion

> We had Wisconsin Breast Cancer Database having 699 records in 11 columns for attributes. 

> Attributes from column indices 2 through 10 have been used to represent instances.
> * Each instance has one of 2 possible classes: benign or malignant.
> * These classes was included as attribute at column index 11

Class distribution was:
> 1. _Benign: 458 (65.5%)_
> 2. _Malignant: 241 (34.5%)_

> After processing data and obtaining analysis from it, we split the dataset into train-test of **70%-30%**. we trained four models. By far, **SVM** model had highest accuracy for training and test data.


[1]: https://archive.ics.uci.edu/ml/machine-learning-databasesbreast-cancer-wisconsin/breast-cancer-wisconsin.data "UCI Machine Learning Repository"
