# Bank-Churn-Survival-Analysis
We have predicted customer churn using the Bank Churn dataset collected from kaggle.
Concepts that we have used:
1. Capturing distribution of numerical variables - Plotting histograms(https://www.youtube.com/watch?v=qBigTkBLU6g)
2. Capturing the distribution for categorical variables - Pie charts(A pie chart shows a part of the whole)
3. Outlier Analysis for numerical variable(univariate Tukey Method): https://www.youtube.com/watch?v=nbNiD76yE8o 
4. Bivariate Analysis: Plotting independent variable against target variable. 
    a. Categorical Target - Categorical Independent Varibale: sns.catplot(kind='count'), sns.barplot(after using groupby along        both categories). https://seaborn.pydata.org/generated/seaborn.catplot.html
    b. Categorical Target - Numerical Independent Variable: sns.violinplot, sns.swarmplot.https://www.youtube.com/watch?v=X0a5HsGcLTY 
5. Pairplot(between two numerical variables): https://www.youtube.com/watch?v=DXj1b28_RdY  
https://www.youtube.com/watch?v=35NWFr53cgA
6. Binning Age Variable: Google Age bins-[18-24, 25-34, 35-44, 45-54, 55-64, 65]https://support.google.com/google-ads/answer/2580383?hl=en
7. Encoding categorical values: LabelEncoder, factorize() method https://www.youtube.com/watch?v=dGIkbH8NqKw https://medium.com/@vaibhavshukla182/want-to-know-the-diff-among-pd-factorize-a8591eb3347d
8. Survival Analysis: https://www.youtube.com/watch?v=fTX8GghbBPc#action=share
https://medium.com/analytics-vidhya/survival-analysis-with-python-fae988ab72cd
