# Bank-Churn-Survival-Analysis
We have predicted customer churn using the Bank Churn dataset collected from kaggle.
Concepts that we have used:
1. Capturing distribution of numerical variables - Plotting histograms(https://www.youtube.com/watch?v=qBigTkBLU6g)
2. Capturing the distribution for categorical variables - Pie charts(A pie chart shows a part of the whole)
3. Outlier Analysis for numerical variable(univariate Tukey Method): https://www.youtube.com/watch?v=nbNiD76yE8o 
4. Bivariate Analysis: Plotting independent variable against target variable. 
    a. Categorical Target - Categorical Independent Varibale: sns.catplot(kind='count'), sns.barplot(after using groupby along        both categories). https://seaborn.pydata.org/generated/seaborn.catplot.html
    b. Categorical Target - Numerical Independent Variable: sns.violinplot, sns.swarmplot.https://www.youtube.com/watch?v=X0a5HsGcLTY 
5. Correlation/Covariance/Pairplot(between two numerical variables): https://www.youtube.com/watch?v=DXj1b28_RdY  
https://www.youtube.com/watch?v=35NWFr53cgA
6. Binning Age Variable: Google Age bins-[18-24, 25-34, 35-44, 45-54, 55-64, 65]https://support.google.com/google-ads/answer/2580383?hl=en
7. Encoding categorical values: LabelEncoder, factorize() method https://www.youtube.com/watch?v=dGIkbH8NqKw https://medium.com/@vaibhavshukla182/want-to-know-the-diff-among-pd-factorize-a8591eb3347d
8. Survival Analysis: https://www.youtube.com/watch?v=fTX8GghbBPc#action=share
https://github.com/zahrael97/Predicting-lung-cancer-survival-time/blob/master/code/Data%20Exploration%20%2B%20Lifeline.ipynb



Note on Survival Analysis:
Survival Analysis in python
Survival Analysis is basically the study of time between two events under consideration.
We basically understand the  pattern in time for different prospective  cohorts under study for same time periods. This technique can be best explained with the help of an example. Suppose, we are studying the time that the people will survive the corona virus attack. Here, the point of origin can be considered as the moment when the patient got corona positive and point of end is when the person succumbs to the disease. Survival Analysis has an upper hand over other methods like t-tests and logistic regression because Survival analysis can deal with censored data.
Censored Data.
Data is said to be censored when one or both of the checkpoints of interest are missing.
There are two types of censoring - 
Right Censoring - Right censoring is when the event of interest does not happen within the time frame of study. For example, when the death/recovery of the subject does not take place within the period of study
Left Censoring - Left censoring is when we do not know the origin checkpoint(event of interest). For example, we do not know when was the subject tested corona positive.
Several Important Functions for survival Analysis :
Survival Function - Survival Function is the probability of survival of a subject more than certain time. It’s value is between 0 and 1.
Hazard Function : Although it has probability in it’s equation but it’s value can be greater than 1 because we have del t in the denominator. It is the probability that a subject will experience an event in a small time interval. This is also known as intensity function. It is a non-parametric statistical technique.
Cumulative Density Function :It is the probability that a subject will survive within the given time period t. It is 1-survival function.
Death Density Function: It is the negative rate of the survival function.


We can not use the root mean squared error method for evaluating the survival analysis technique.
Three techniques for evaluating the survival analysis are :
Concordance Index - It is the ratio of concordant pairs to total number of pairs.
Brier score  
Mean absolute error.

Kaplien Mier Estimate : It is used to predict the survival function from the lifetime data. It is a non-parametric statistical technique.
Proportional Hazard is a type of survival model in statistics. This model maps the time elapsed before happening of the event to the various factors related to the happening of that event.
By taking a certain medicine the time before death becomes twice of what it was before similarly if we half the dosage the time before death decreases upto two times.

