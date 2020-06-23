# Real-Estate-Price-Prediction
Predicting the real estate price for properties and houses across the city of **Bengaluru, India.**
The project mainly has two parts:
## Data Science
## Machine Learning
###### Data Science
- The first step is typical data science work where we take a data set from Kaggle called ‘Bengaluru House price data’.
- We will perform some extensive data cleaning work on it to ensure that it gives accurate results during prediction.
- This jupyter notebook entitled ‘Real Estate.ipynb’ is where we perform all the data science related work. 
- As the jupyter notebook is self-explanatory I shall briefly touch upon the concepts that I have implemented. 
- Our dataset requires a lot of work in terms of data cleaning. 
- In fact, 70% of the notebook is all about data cleaning where we drop empty rows and remove unnecessary columns that won’t help in prediction.

Next step, Feature Engineering which is the process of extracting useful and important information from the dataset that will contribute the most towards a successful prediction.
The final step is handling outliers.
- Outliers are anomalies that cause an enormous amount of damage to data and prediction. 
- There is a lot of things to understand from the dataset logically to detect and remove these outliers.
- Again, all of these have been explained in the jupyter notebook.
- In the end, the original dataset which had almost 13000 rows and 9 columns are reduced to almost 7000 rows and 5 columns.
###### Machine Learning
The final data obtained is subjected to a machine learning model. 
- We will mainly use K-fold Cross Validation and GridSearchCV technique to perform hyper parameter tuning to obtain the best algorithm and parameters for the model.
- Turns out linear regression model gives the best results for our data with a score above 80% which is not bad.
- Now, our model needs to be exported into a pickle file (Bengaluru_House_Data.pickle) which converts python objects into a character stream. 
- Also, we need to export the locations(columns) into a json(columns.json) file to be able to interact with it from the frontend.
Server
