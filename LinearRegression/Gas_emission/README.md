# Machine Learning Model build up for a Linear Regression containing gas emmissioin dataset

# Own Article link:
https://www.linkedin.com/posts/chiranjit-pathak-2261892a_linear-regression-with-feature-engineering-activity-6751702790420078592-SMnT



<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/LinearRegression/Gas_emission/Pics/pic1.jpg?raw=true"/>


<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/LinearRegression/Gas_emission/Pics/pic3.png?raw=true"/>



## Table of Content

1. [Problem Statement](#section1)<br>
2. [Data Loading and Description](#section2)<br>
3. [Exploratory Data Analysis](#section3)<br>
4. [Training and testing the Model](#section4)<br>
    - 4.1 [Splitting data into training and test datasets](#section401)<br>
    	- 4.1.1 [Feature Selection using using Correlation Statistics](#section4011)<br>
    	- 4.1.2 [Feature Selection using Mutual Information Theory](#section4012)<br>
    - 4.2 [Linear regression in scikit-learn](#section402)<br>
    	- 4.2.1 [Model with all features](#section4021)<br>
    	- 4.2.2 [Model Built Using Correlation Features](#section4022)<br>
    	- 4.2.3 [Model Built Using Mutual Information Features](#section4023)<br>
    	- 4.2.4 [Tune the Number of Selected Features : GridSearch](#section4024)<br>
    - 4.3 [Interpreting Model Coefficients](#section403)<br>
    - 4.4 [Using the Model for Prediction](#section404)<br>   
5. [Model evaluation](#section5)<br>
    - 5.1 [Model evaluation using metrics](#section501)<br>
    - 5.2 [Model Evaluation using Rsquared value.](#section502)<br>
6. [Conclusion](#section6)<br>


## 1. Problem Statement

The dataset can be well used for predicting __turbine energy yield (TEY)__ using __ambient variables as features__

In our role as __Data Scientist__ we are asked to suggest.

- We want to find a function that given input as parameters and will __predicts the output__.

- Which __features__ contribute more to __TEY__?

- Visualize the __relationship__ between the _features_ and the _response_ using plots.


## 2. Data Loading and Description

Source:

https://archive.ics.uci.edu/ml/datasets/Gas+Turbine+CO+and+NOx+Emission+Data+Set


### Data Set Information:

The dataset contains __36733 instances__ of __11 sensor measures__ aggregated over one hour (by means of average or sum) from a gas turbine located in __Turkey's north western region__ for the purpose of studying __flue gas emissions__, namely __CO and NOx (NO + NO2)__. 

The data comes from the same power plant as the dataset used for predicting hourly __net energy yield__. 

By contrast, this data is collected in another data range __(01.01.2011 - 31.12.2015)__, includes gas turbine parameters __(such as Turbine Inlet Temperature and Compressor Discharge pressure)__ in addition to the __ambient variables__. 

Note that the dates are not given in the instances but the data are sorted in chronological order. See the attribute information and relevant paper for details. Kindly follow the protocol mentioned in the paper __(using the first three years' data for training/ cross-validation__ and the __last two for testing)__ for reproducibility and comparability of works. 

The dataset can be well used for predicting __turbine energy yield (TEY)__ using ambient variables as features.


### Attribute Information:

The explanations of sensor measurements and their brief statistics are given below.

<img src="https://github.com/pathakchiranjit/Machine-Learning/blob/main/LinearRegression/Gas_emission/Pics/variable_1.JPG?raw=true"/>
