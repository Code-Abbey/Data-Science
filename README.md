# Data-Science


This is a classification task. 
The file “Flight.csv” contains the following data: 
Month 
Month number (only year 2018)
DayOfWeek 
1 (Monday) – 7 (Sunday)
AirTime 
Time in air in minutes
Distance 
Flight distance in miles 
TaxiIn 
Time between landing and reaching the gate in minutes
TaxiOut 
Time between leaving the terminal gate and taking off.
Delay 
late (arrival delay >= 15 min), ontime (arrival delay < 15 min)
jfk_origin 
1 (start or landing JFK), 0 (other)



The variable “Delay” is the target! 
Perform the following tasks / answer the following questions in a jupyter notebook. 
1) Load the file “flights.csv” in a dataframe with the name df 
2) How many rows and how many columns does the dataframe have? 
Write an answer sentence! 
3) Cast the variable “DayOfWeek” to datatype “category”. 
4) Create a bar chart of the variable " DayOfWeek". 
Interpret this bar chart (1-2 sentences) 
5) Create a histogram of the variable "AirTime". 
Interpret the histogram (2-3 sentences). 
6) Run the following line of code: 
sns.scatterplot(data=df, x='AirTime', y='Distance',hue='Delay'); Interpret this scatterplot (3-4 sentences) 
7) Create the correlation matrix of df. You can use the following code: 
pd.options.display.float_format = '{:,.2f}'.format 
corr_matrix = df.corr(numeric_only=True) 
corr_matrix 
Interpret the correlation value between “AirTime” and “jfk_origin”. 
8) Dummy Enode all categorials. 
(Only DayOfWeek is a categorial) 
9) Create the feature matrixes X_train and X_test (without the target) 
and the targets y_train and y_test. 
The ratio of train to test should be 75%:25%. 
10) If you use the notebook “Classification-Notebook-V03.ipynb: 
In section 8, define the positive and negative class as: 
class_pos = 'late' 
class_neg = 'ontime' 
11) Perform a logistic regression, calculate the confusion matrices and the accuracy (for training and testing). Interpret the calculated accuracies. 
Test data: what is the probability that an on-time airplane was estimated to be on time? 12) Perform a decision tree classifier without regularization (default values of the parameters). Interpret the calculated accuracies. 
13) Bonus Points: What do you recommend for a better classification? 
Upload your Jupyter notebook on ecampus (10:45).
