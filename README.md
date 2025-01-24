## Title - Predictive Maintainance Analysis

### Discription of Project

- This project is related to a mechanical industry, Sometimes in industries unexpected machine failures occurs due to    improper handling, power cutoff, faulty     instrument, improper machine parameters given by operator. 
- By analysing and finding insights from the Dataset of drilling tool which is used on lathe machine in mechanical 
  industry we created a model using a machine learning algorithm which predict if machine will get failure or not.

### Future scope This Project 

- By using this model we can improve the productivity of companies.
- We can easily predict  machine will fail or not before start the production by providing input parameters.
- Prevent the machine from failures.
- Improves the safety features from accidents.  
- Language used (PYTHON, EXCEL)

### Data Information
- After looking at the dataset, we can assume that the data is about the drilling tool used in a lathe machine.

- The columns consist values of:
     1. Air temperature in Kelvin (K)
     2. Process temperature in Kelvin (K)
     3. Rotational speed in Rotation per minute (RPM)
     4. Torque in Newton meters (Nm)
     5. Tool wear in minutes (min)

 - Type column is given to represent the type of product with respect to its quality. 
   L, M and H are for Low, Medium and High quality products respectively.

 - ProductID consisting of a letter L, M, or H for low (50% of all products), medium (30%), and high (20%) as product quality variants and a variant-specific 
   serial number.

 - The target column is the output of machine, if it is failing or not.
   0 represents no failure whereas 1 represents that failure has occured.

 - An additional column of Failure Type is given so that we can understand what type of failure is occuring.
   
### Input Columns and Output column

1. Air temperature in Kelvin (K)
2. Process temperature in Kelvin (K)
3. Rotational speed in Rotation per minute (RPM)
4. Torque in Newton meters (Nm)
5. Tool wear in minutes (min)
6. Type
7. Failure Type
8. Target ---> Output column
   
### libraries used in this project

- numpy
- pandas
- matplotlib
- seaboran
- ScikitLearn
- Filter warning
  
### Data Insights

 1. The data contain no null values and also having categorical columns.

 2. The data is normally distributed because the value of mean and median(50%) is close to each other
    so there is no need to skewness removal.

 3. The the ratio of machine failure is less than as compare to no failure and so there is imbalance in two columns. 

 4. Type of Failure -
    
    - Heat Dissipation Failure : The failure that occurs due to overheating of the tool.
    - Power Failure : The failure occuring due to power cutout.
    - Overstrain Failure : Failure because of excessive strain on the tool.
    - Tool Wear Failure : Failure due to tool wear and tear that happens after excessive use of tool.
    - Random Failures : Random Failures can be any failure whose cause can't be assessed or any human error.
    
 5. Most of time the machine get failed due to Heat Dissipation Failure and after that Power Failure then Overstrain Failure and last Tool Wear Failure.

 6. From our total products 60% are low quality products and 30% are medium quality products then 10% are high quality products.

 7. Rotational speed [rpm], Torque [Nm], Tool wear [min] are highly affecting to our Target column.

### Used Model 

 - Logistic Regression.
 - KNeighbors Classifier 
 - DecisionTree Classifier
 - RandomForest Classifier

### Model Building
 - Here we created a function to check which Machine Learning Algorithm will be the best fit for our model and We will select the one with highest accuracy.
   
### Model Evaluation
  - classification_report
  - accurary
  - precision
  
### Train Test score 
  - Hyperparameter Tunning
   
### Final Model Deployment
  - Model with well suitable and with high accuracy

### Model Testing
 
  - using sample values
  
  1. Example:-
  
  - Type = M
  - Air temperature [K] = 298.2
  - Process temperature [K] = 308.5
  - Rotational speed [rpm] = 2678
  - Torque [Nm] = 10.7
  - Tool wear [min] = 86
  - Target = 1

  2. Example:-

  - Type = H
  - Air temperature [K] = 298.4
  - Process temperature [K] = 308.9
  - Rotational speed [rpm] = 1782
  - Torque [Nm] = 23.9
  - Tool wear [min] = 24
  - Target = 0
    
### Prescriptive Analysis
   After studying the dataset, we can see that machine failure is mainly occuring because of 3 reasons:
   1. Improper rotational speed of the spindle.
   2. Torque not maintained as per the requirement.
   3. High tool wear.

### Measures to take in order to avoid failure.
    1. User must set the rotational speed properly. Not too high and also not too low.
    2. User should not set the torque too high or too low. Torque should be set as per the tool requirement.
    3. User should not use the same tool for long period of time. Since tools may wear due to excessive usage.
    4. High quality and medium quality products should be used more frequently.
    5. Overheating of tool must be avoided by constantly providing coolant to the tool. 
    6. Secondary power input shoould be provided in case of power failure
