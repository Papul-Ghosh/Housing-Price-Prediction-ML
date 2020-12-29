# ML-Housing-Price
 
**Machine Learning Housing Price prediction with Scikit Learn**
 
 The task is to predict median house values in California districts, given a number of features from these districts.
 
 Data source: raw.githubusercontent.com/ageron/handson-ml2/

In this project, the included steps are:

1. Get the data
2. Discover and visualize the data to gain insights
3. Data Preparation
4. Select and train a model
5. Fine-tune the model


**1. Get the data:**

Shape of dataset: (20640, 10)

Length of Train set: 16512

Length of Test set: 4128

stratified sampling is included here


**2. Discover and visualize the data to gain insights:**

New features added: "rooms_per_household", "bedrooms_per_room", "population_per_household"

Correlation (housing.corr()) between all the features with "median_house_value" is checked to find strong insights.


**3. Data Preparation:**

It includes:

filling NaN values with medians

Converting text features to numbers (OrdinalEncoder class)


**4.Select and train a model:**

Models implemented: Linear Regressor, Decision Tree Regressor, Random Forest Regressor, Support Vector Regressor

Cross validation is implemented to improve model performance.


**5. 5. Fine-tune the model:**

Cross validation score is used to calculate the RMS error

GridSearchCV class is used to fine tune the hyperparameters.

The optimal rms error is found by the Random Forest Regressor and value is: 47730.22690385927

The mean value for median_house_value in the test set is: 205500.309593

