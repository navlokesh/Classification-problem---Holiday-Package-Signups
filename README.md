# Classification-problem---Holiday-Package-Signups

We will check how to perform EDA, build different models and compare them to decide which model to use.

A data by a tour and travel agency which deals in selling holiday packages is available. Data provides details of 872 employees of a company. Among these employees, some opted for the holiday package and some didn't. Lets us analyze and predict whether an employee will opt for the package or not on the basis of the information given in the data set. Also, let us find out the important factors on the basis of which the company will focus on particular employees to sell their packages.

## Exploratory Data Analysis:
Univariate and bivariable data analysis was done using histograms, boxplots, null value checks, pairplots, heatmaps and other statistical values from the data.

From the Pairplot and the heatmap, below is the observation of correlation between the variables:
• The variable Salary is positively correlated with Education with correlation of 0.33, which is not a high number
• There is negative correlation between number of young children and age variables
• Apart from these there is very minimal correlation between rest of the variables
The output variable Holiday package and one of the independent variable Foreign are in object data type. These will be converted to integers by encoding, in later parts of the project.

## Data Split and Model Building:
Catergorical variables were converted to numerical using encoding techniques and data was split into training and test sets.

Training data was used to build the model using Logistic Regression and Linear Discriminant Analysis algorithms.

## Model Performance:

Model evaluation was done using various metrics such as Accuracy, Confusion matrix, ROC_AUC graphs, etc.

From the performance metrics, we saw that the results of LDA is better than logistic regression.
The model built on LDA has better roc_auc_score and accuracy score when compared to logistic regression.
The recall and f1 scores for Logistic regression is too low when compared to LDA.
Hence, we can say that the model build on LDA is performing better whne compared to logistic regression.

## Inference:

The variables in the dataset doesn’t seem to be having high correlation with the output variable. The company may have to consider concentrating on other attributes which could potentially have higher correlation with the output factor.
The output variable is having positive correlation of 0.25 with the column ‘Foreign’. So, concentrating on these employees could have better conversion rate when it comes to buying the holiday package.
When is comes to choosing the model, Linear Discriminant Analysis seems to be performing better when compares to Logistic regression.
