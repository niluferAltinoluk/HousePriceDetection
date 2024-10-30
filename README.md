## Project Overview

In this project, we did a machine learning, data science project with the help of Python libraries. Our project is designed to predict house prices.

## Python Packages Used
* Pandas: For data manipulation and analysis.
* NumPy: For numerical operations.
* Seaborn: For data visualization.
* Scikit-learn: For machine learning and data mining.
* Matplotlib: For data visualization.

## Data

* Id: Our data ids
* Area: The total area of the property, typically measured in square feet or square meters. This includes both indoor and outdoor space. int
* Bedrooms: The number of bedrooms in the property. int
* Bathrooms: The number of bathrooms in the property. int
* Floors: The number of floors in the property. int
* YearBuilt: The year the property was constructed. int
* Location : The geographic location of the property.Categorized  as DownTown, Suburban, Urban, or Rural. 
* Condition : The overall condition of the property  categorized  as poor, fair, good, or excellent.
* Garage	: Information about the property's garage. yes/no
* Price : The asking price or sale price of the property. int


## Code structure

1. We stored the data as df
2. We drop our id column.
3. We make visualtion as
   * Location/ Price boxplot for Comparing Price Distribution of Different Locations
   * Condition/ Price boxplot with hue Garage. It helps to understand those informations. Visual understanding of how the condition of homes and whether they have a garage affects home prices. Comparing price distributions of houses in different situations and garage combinations.
   * Floors/ Price boxplot with hue Location. It helps to understand those informations. Want to analyze how the number of floors affects house prices in different locations. Distribution of the Number of Floors of Different Locations.
   * Bedroom/ Price boxplot with hue Location as similar reasons like Floors/ Price boxplot with hue Location.
   * Bathroom/ Price boxplot with hue Location as similar reasons like Floors/ Price boxplot with hue Location.
4. We divided the features in our dataset into two categories: numerical and categorical.
5. We normalized our numeric features in a DataFrame using a Min-Max scaler.
   * We wanted to scale our numerical data and obtain more accurate values.
   * Since all our numerical features in the data set are positive and within a certain range, we preferred the min-max scaler.
6. Using one-hot encoding, we converted categorical data into numerical data by creating a new binary feature for each category.
   *We chose it because there is no order among the categories.
7. We divided the data into two to use in our machine learning model.
8. We randomly split the dataset into 20% testing and 80% training, and assigned the features (X) and target variables (y) of each cluster to separate variables.
9. We created an instance of the linear regression model from the scikit-learn library and assigned it to a variable called "model".
    *Linear regression is one of the most basic and common statistical methods used to model the relationship between two or more variables.
10. We fit our model.
11. We created y_pred to enable us to make predictions on new, previously unseen data using a machine learning model we've previously trained.
12. We evaluated the performance of the model with MSE.
   *Mean Squared Error (MSE) is a common metric used to evaluate the performance of regression models. It measures the average squared difference between the predicted values and the actual values.

## Results and evaluation

In our project, we saw that house prices in certain locations were largely the same. We examined the connection between the home condition and the garage. In the following examples, we obtained outputs on these issues by visualizing our rooms. My comment on the bedroom price chart, which is a remarkable chart, was that the location of the house affects the number of bedrooms and the Suburban location has fewer bedrooms compared to the others. Although the number of rooms was a factor in the price point, those with a lower number of bedrooms and bathrooms could be found at higher levels.


## Future Work

We can make more visualizations to make more effective interpretations on our data set. We can make use of multiple visualizations. We can choose different models for our model. With the help of Model Tuning, we can maximize the performance of the model. We can achieve better results by combining the predictions of different algorithms.
We can also build more effective models with the help of the tensorflow library. Our data set consists of 10 columns, and in this data set we can compare the results with the algorithm methods we use for larger data sets.








