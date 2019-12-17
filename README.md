# studentpref-lr-svm-nb-dt

# Description of the problem

-The dataset provided consist of data of 60 students and their performance when taught by a few different method by their tutors.
-Here, we will perform analysis on the ”outcome variable” to help us understand it better.
-Here the “outcome” variable is the student’s change on standardized score after training
-Various variables in the dataset add to the output of the “outcome” variable, which are provided to us with its relevant information.
-We will be running a few algorithms and check which model fits the dataset well, and if it can generate some insights addressing to our problem.

# Methodology

-There are various types of methodologies we could use to tackle this problem and generate some useful insights.
-Here we will be using Logistic Regression, Support Vector Machines, Naïve Bayes and Decision Trees.
-Lets us look at what these algorithms do and what are they based on:
  Logistic Regression: This type of regression is mainly used when the dependent variable is binary in nature. 
  Support Vector Machines: This algorithm is used when we need to classify a variable, it uses a hyperplane to separate the two classifications.
   Naïve Bayes: This algorithm is based on the Bayes theorem which classifies the data by the help pf probability.
  Decision Tree: This algorithm uses a structure of nodes which are known as branches to depict all the outcomes which are possible.
  
  # Exploratory Data Analysis
  
-Now we will perform basic statistics and exploratory data analysis on the dataset to understand the distribution of the data better.
-First, we see that there is no missing data in any variables.
-“Method” is a categorical variable so the basic statistics may not give us a lot of information.
-Same goes with the “outcome” variable as it is a categorical variable too.
-Variables like “ability” and “prvpref” show that there may be a correlation between the two as “ability” is the forecasted score based on current math knowledge and “prvscore” is the student’s score on a standardized math test a year ago.
-The statistics shown of the variables “satis” and “time” does not show a lot statistics which is eye catching, we could see its effects on the “outcome” variable later to see its impacts.
-The highest standard deviation is shown in the variable “ability” with 11.295854.

# Confusion Matrix, Classification, Key Insights

-Now we will talk about the Confusion Matrix, Classification, and its Key Insights.
-When we look at the Logistic Regression confusion matrix, the “True negative box shows “1” which is very low for making any predictions.
-The glaring part of it is the accuracy which is quite low at 42%
-It also shows that the data of “1” which is “positive change in prvscore” is unbalanced as the precision, recall and f1-score are 0.25, 0.20 and 0.22, respectively.
-The macro average and the weighted macro averages are not up to a level where we can adopt this algorithm for our analysis.

-When we look at the Support Vector Machine’s confusion matrix, it is exactly like the confusion matrix of Logistic Regression.
-This is possible because both the algorithms are based on classification of the data.

-When we look at the Naïve Bayes confusion matrix, the False positive box shows “1” which is very low for making any predictions.
-The accuracy is a lot higher than what we obtained for Logistic Regression and Support Vector Machines at 67%.
-It also shows that the recall score if 1 is very low at 0.40 as it is computed using the True Positive and False Positive Values, as the False Positive value is low at “1”, it is understandable that we obtain 0.40 here.
-The macro average and the weighted macro averages are not up to a level where we can adopt this algorithm for our analysis but still a lot of better than the other two algorithms we computed.

-When we look at the Decision tree confusion matrix, the False negative and True Negative shows “2” which is very low for making any predictions.
-The accuracy is a lot higher than what we obtained for Logistic Regression and Support Vector Machines at 58% but still a lot lower than Naïve Bayes.
-There may not be any glaring differences here, the values of precision, recall and f1-score are normal in terms of accuracy we obtained.

# Recommendation, Improvements

-Looking at all the output of the algorithms and its confusion matrix, we can say that out of the 4 algorithms, only the Naïve Bayes algorithm is the one we could consider to pick out of them all with 67% of accuracy.
-The Logistic Regression, SVM and Decision Tree do not qualify as we can see that they are not able to have good accuracy and have a poor fit in terms of the dataset.
-The improvements here could be done that we could collect more data so that we have ample chances to predict either side of the categories and not just one.
-If there is more data included, we could see improvements for not only Naïve Bayes but all other algorithm outputs too.
-Naïve Bayes is surely a time taking model but looking at the size of the dataset at 60, it seems to be the best bet out of them all.
