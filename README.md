# Sparkify_PySpark
Predict user churn with Spark.


### Project motivation:

The project is about predicting customer churn. It is a fictional app similar to spotify. It predicts the churn rate of customers based on different features.

### Installation:

Jupyter Notebook runs with Python 3.

If following libraries aren't installed already, run <strong>"pip install <package_name>"</strong> or <strong>"conda install <package_name>"</strong> in your command line.

-pyspark

-pandas

-matplotlib

-seaborn  <strong> Due probably updating issues it is possible that seaborn doesn't work completely. Therefore, I included an install command to ensure it executes all neccesary functions, objects, etc...</strong>


### File description:

#### Data
Because of github's upload size constraint, I have splitted the json data into 6 single files. In order to run the app, follow these steps.

1. Create new file and name it "mini_sparkify_event_data.json"
2. Copy the content of the singles files into "mini_sparkify_event_data.json" by ascending order.

#### Code
"Sparkify.ipynb" contains all the necessary code to run the app.

### Results:

I transformed features to numerical values and standardized it. Following 3 algorithms has been used:

#### 1. Gradient Boosted Tree:   
Accuracy: 0.9884               
F1 Score: 0.9883              
Training time: 574.63 seconds

#### 2. Logistic Regression: 
Accuracy: 0.8368    
F1 Score: 0.7625    
Training time: 191.61 seconds

#### 3. Random Forest Clasifier: 
Accuracy: 0.8859    
F1 Score: 0.8588    
Training time: 262.85 seconds

#### Hypertuned gradient boosted tree:
F-1 score:
0.9952

### Future Improvements:

Training the model on the large dataset would help a lot. Extract and use more features, that would lead to a more robust model. Random over- or down-sampling could be applied in order to get a more balanced dataset. 

### Blog Post:

The Blog Post can be found on https://medium.com/@danny.kirchner/predicting-customer-churn-rates-b3fa0e9621ed
