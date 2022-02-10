# Rider-Driven-Cancellation-Prediction
---
### About the Project :

- Techstack: Machine Learning, Scikit-Learn, Python
- A model that can predict rider-driven cancellation in advance. 
- Made using data consisting information of orders and riders.
- Data was processed and different algorithms were used for classification.

### Data Processing :

- In order to not repeat the process all over again, we concatenate train and test for processing.
- Checked for column mismatch and deleted columns that were not present in either of the sets.
- Checked for null values and dropped columns that had a very high count.
- Converted Time-based columns to DateTime and split the necessary parts of date and time into seperate columns.
- Calculated difference between time for certain actions and stored the results in a separate column.
- Used alloted, delivered and undelivered columns to form one single column representing the three aforementioned.

### Pipeline and Modelling :

- Used sklearn to make a pipeline which imputes the 'median' value for null in columns.
- Split the dataset into X and y and further into their train and test subsets using sklearn.
- Tried different classification algorithms (LogisticRegression, DecisionTreeClassifier, etc.) and evaluted the results.
- Once the model was ready, the pipeline and model were used again on the test set to make final predictions.
