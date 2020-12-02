# Machine Learning Model build up for a Binary Classification containing Machine Failure dataset


<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Machine_Failure/Pics/predictive_model.jpg?raw=true" />


As Industry 4.0 continues to generate media attention, many companies are struggling with the realities of AI implementation. Indeed, the benefits of predictive maintenance such as helping determine the condition of equipment and predicting when maintenance should be performed, are extremely strategic. Needless to say that the implementation of ML-based solutions can lead to major cost savings, higher predictability, and the increased availability of the systems.

<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Machine_Failure/Pics/prediction.png?raw=true"/>

---

In predictive maintenance scenarios, data is collected over time to monitor the state of equipment. The goal is to find patterns that can help predict and ultimately prevent failures.

<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Machine_Failure/Pics/reliable%20plant.gif?raw=true"/>

<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Machine_Failure/Pics/ptof1.png?raw=true"/>



## Table of Contents

1. [Problem Statement](#section1)<br>

2. [Data Loading and Description](#section2)<br>

3. [Preprocessing](#section3)<br>
    - 3.1 [Importing packages](#section301)<br>
    - 3.2 [Label Encoding for Categorical data](#section302)<br>
    - 3.3 [Binary Class Identification : Imbalanced dataset](#section303)<br>
    - 3.4 [Feature Corelations](#section304)<br>

4. [Handling Imbalanced data](#section4)<br>
    - 4.1 [Train & Test split](#section401)<br>
    - 4.2 [SMOTE : Oversampling technique adopted on Train data](#section402)<br>
  
5. [Logistic Regression](#section5)<br>
    - 5.1 [Build Model](#section501)<br>
    - 5.2 [Prediction using Model](#section502)<br> 
    - 5.3 [Model Evaluation](#section503)<br> 
    
6. [Decision Tree : Gini](#section6)<br>
    - 6.1 [Build Model](#section601)<br>
    - 6.2 [Prediction using Model](#section602)<br> 
    - 6.3 [Model Evaluation](#section603)<br>
	
7. [Decision Tree : Entropy](#section7)<br>
    - 7.1 [Build Model](#section701)<br>
    - 7.2 [Prediction using Model](#section702)<br> 
    - 7.3 [Model Evaluation](#section703)<br>
	
8. [Random Forest : Gini](#section8)<br>
    - 8.1 [Build Model](#section801)<br>
    - 8.2 [Prediction using Model](#section802)<br> 
    - 8.3 [Model Evaluation](#section803)<br>
	
9. [Random Forest : Entropy](#section9)<br>
    - 9.1 [Build Model](#section901)<br>
    - 9.2 [Prediction using Model](#section902)<br> 
    - 9.3 [Model Evaluation](#section903)<br>
	
10. [Decision Tree with Class weight and Entropy](#section10)<br>
    - 10.1 [Build Model](#section1001)<br>
    - 10.2 [Prediction using Model](#section1002)<br> 
    - 10.3 [Model Evaluation](#section1003)<br>
	
11. [RandomSearchCV on RF](#section11)<br>
    - 11.1 [Build Model](#section1101)<br>
    - 11.2 [Prediction using Model](#section1102)<br> 
    - 11.3 [Model Evaluation](#section1103)<br>
	
12. [Model Evaluation among all the employed model](#section12)<br>
    - 12.1 [Precision-Recall Curve and Classification Report](#section1201)<br>
    - 12.2 [ROC-AUC Curve and compare against no skill model](#section1202)<br>
    - 12.3 [Probability Value comparison of test dataset among all models](#section1203)<br>
	
13. [Cross Validation and Prediction with selected model](#section13)<br>

14. [Conclusion](#section14)<br>

