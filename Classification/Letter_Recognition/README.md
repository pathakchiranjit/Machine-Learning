# Machine Learning Model building for Letter Recognition dataset using multiclass classification


<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Letter_Recognition/Pics/l10.gif?raw=true" />


<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Letter_Recognition/Pics/l11.gif?raw=true" />

Letter recognition using machine learning algorithm is practised as a case study across the globe.

<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Letter_Recognition/Pics/l4.jpg?raw=true"/>


## Table of Contents

1. [Problem Statement](#section1)<br>

2. [Data Loading and Description](#section2)<br>

3. [Preprocessing](#section3)<br>
    - 3.1 [Importing packages](#section301)<br>
    - 3.2 [Exploratory Data Analysis](#section302)<br>
    - 3.3 [Feature Selection](#section303)<br>

4. [Train-Test Split](#section4)<br>
  
5. [OneVsRest Classifier : SVC - RBF](#section5)<br>
    - 5.1 [Build Model](#section501)<br>
    - 5.2 [Model Evaluation](#section502)<br>
	
6. [OneVsRest Classifier : RandomForest](#section6)<br>
    - 6.1 [Build Model](#section601)<br>
    - 6.2 [Model Evaluation](#section602)<br>
	
7. [OneVsRest Classifier : LogisticRegression](#section7)<br>
    - 7.1 [Build Model](#section701)<br> 
    - 7.2 [Model Evaluation](#section702)<br>
	
8. [OneVsRest Classifier : Naive Bayes](#section8)<br>
    - 8.1 [Build Model](#section801)<br> 
    - 8.2 [Model Evaluation](#section802)<br>

9. [OneVsRest Classifier : SVC - Linear](#section9)<br>
    - 9.1 [Build Model](#section901)<br>
    - 9.2 [Model Evaluation](#section902)<br>

10. [Model Evaluation among all the employed model](#section10)<br>
    - 10.1 [Precision-Recall Curve among models](#section1001)<br>
    - 10.2 [Confusion Matrix and Classification Report](#section1002)<br>
	
11. [Cross Validation and Prediction with selected model](#section11)<br>

12. [Conclusion](#section12)<br>


### 1. Problem Statement

The objective is to __identify__ each of a large number of __black-and-white__ rectangular __pixel displays__ as one of the __26 capital letters__ in the English alphabet

<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Letter_Recognition/Pics/l1.jpg?raw=true" />

### 2. Data Loading and Description

Source of the data:

https://archive.ics.uci.edu/ml/datasets/letter+recognition


- The character images were based on __20 different fonts__ and each letter within these 20 fonts was randomly distorted to produce a file of __20,000 unique stimuli__. Each stimulus was converted into __16 primitive numerical attributes (statistical moments and edge counts)__ which were then scaled to fit into a range of integer values from 0 through 15. 
- We typically train on the first 16000 items and then use the resulting model to predict the letter category for the remaining 4000. 
- Below is a table showing names of all the columns and their description.

<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Letter_Recognition/Pics/l2.jpg?raw=true"/>


<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Letter_Recognition/Pics/l16.png?raw=true"/>

<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/Classification/Letter_Recognition/Pics/l9.jpg?raw=true"/>
