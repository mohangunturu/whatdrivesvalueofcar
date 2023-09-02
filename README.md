# What drives the price of a used car?

I have used CRISP-DM model for analysis of the data,building a model, evaluating the model with cross validation.
The steps are below.

### Business Understanding

### Background:
Used car sales dealership wants to know what drives the price of the car so that they can appropriately price the car to gain buy or sell the used cars.
### Business Objectives: 
Identify what are the features or attributes that drives the price of the car. Set the price for the car for sale based on findings.
### Business Success Criteria: 
Set the car price appropriately either for buying or selling to gain maximum profitability
### Access Situation: 
We need to identify the dataset that contains several features of any given car such as make, model, odometer reading, condition, color, location etc.
### Risks: 
There may be a possibility of the data is not accurate or insufficient or not useful
### Costs/Benefits: 
The cost to run analysis to give the price range for any given car so that the delarship can sell appropriately.
### Data Mining/Success goals: 
Identify data, collect the data elements, and samples for various sources. Here the data set is given.
### Project Plan: 
Prepare a project plan to collect data, resources, data analysis,  modelling, deployment and monitoring.
### Tools: 
Linear Regression, Python, Jupyter notebook, and several algorithms, validations etc.


### Data Understanding

### Collect Initial Data:
Run several campaigns to collect the data. Here we got the dataset, so we are not doing anything.
### Describe Data:
The data has 426880 data points with 18 features with several data types.
### Explore Data: 
Explore the data with techniques to identify what features are important using several plots, detecting outliers, treat missing values,data type changes, data cleansing, and null checks etc.
### Verify Data Quality: 
Inspect the data for quality, consistency, range, and length etc.

## Data Preparation

### Data Cleaning:
Cleaned the data, checked for nulls,categorized the data of non-numeric columns using several encoding techniques.

Prepared correlation matrix for identifying the relationship between these variables

Built PCA components to see what are the main features and how it is impacting the price of the used car.

## Modelling & Evaluation

Used several techniques to build and evaluating the unexplainability.
## Summary of Model Performance and Valdiation

There are several models that I have applied to investigate whick model will be best fit.I have performed PCA analysis, Linerar Regression, Polynomical features and also evaluated with GridSearch. Also performed cross validation with several techniques

Results summary:

Linear Regression

Y Test MSE: 168754271.59119785
Y Train MSE: 3728939.701984654
R-squared (Coefficient of Determination): 0.15649912415780498

Linear Regression with Polynomial Features Degree 1:


Y Test MSE: 168766169.0436156
Y Train MSE: 3728933.906139738
R-squared (Coefficient of Determination): 0.15643965596514808

Grid Search Evaluation with n=5

Y Test MSE: 167992201.59929857
Y Train MSE: 3729488.081120623
R-squared (Coefficient of Determination): 0.16030825265902182


With 85% explainable model seems to be good with 15% unexplainability from the model


Next Steps:
I would like evalutate further the model on some of the features how we can encode better and run other techniques to see if we can improve the model further to explain the possiblity of reamining 15%.

I would like to create model with only the columns that has more importance and see how these models perform and perdict with more accuracy.



## Deployment
Now that we've settled on our models and findings, it is time to deliver the information to the client. You should organize your work as a basic report that details your primary findings. Keep in mind that your audience is a group of used car dealers interested in fine tuning their inventory.

## Final Report:
Based on PCA analysis the used car dearship need consider the vehicles that has the below features. The used car prices are driven by model,type,drive,cylinders,region,state,fuel,year,made by ford,paint_color,transmission and condition.

Using Linear regression we are only unable to explain 15% of variance in the model, means with 85% accuracy it will predict.

We can further narrow down what are the top features that drives used car price as a next step.