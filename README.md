# Real Estate Analysis Project

## Project Background

In today's market, more people are interested in buying homes or learning about real estate for investment. However, real estate is complex, and even experienced buyers can struggle to track market trends and assess property values accurately. Websites like Real Estate and Allhomes offer information on housing, but they primarily focus on existing properties. None provide tools for estimating the value of a new home based on personal criteria or predicting the profitability of real estate investments.

To address these gaps, Team 23 – KT Rolster developed a real estate website using Machine Learning to offer smarter, more accurate data processing. The site is user-friendly and caters to both individual buyers and investors. However, our primary target audience is home buyers and real estate investors. Home buyers can estimate home values based on factors like location and amenities, while investors can categorize properties into premium, mid-range, or affordable segments to assess investment potential more effectively.

## Techniques Introduced

### 1. Regression

Regression analysis is a statistical method used to understand the relationship between a dependent variable and one or more independent variables. In this project, we use regression to predict the price of a house based on various features such as location, size, and amenities.

#### Model: Random Forest Regressor

The Random Forest Regressor is an ensemble learning method that operates by constructing multiple decision trees during training and outputting the mean prediction of the individual trees. It is robust to overfitting and provides high accuracy.

### 2. Classification

Classification is a supervised learning technique used to categorize data into predefined classes. In this project, we use classification to categorize properties into different segments such as premium, mid-range, or affordable.

#### Model: Random Forest Classifier

The Random Forest Classifier is an ensemble learning method that constructs multiple decision trees during training and outputs the mode of the classes (classification) of the individual trees. It is effective for handling large datasets with higher dimensionality.

### 3. Clustering

Clustering is an unsupervised learning technique used to group similar data points together. In this project, we use clustering to identify patterns and group similar properties based on their features.

#### Model: K-Means

K-Means is a popular clustering algorithm that partitions the data into K clusters, where each data point belongs to the cluster with the nearest mean. It is simple and efficient for large datasets.

## Usage Guide

### Library Require:

1. pandas: For data manipulation and analysis.
2. numpy: For numerical operations.
3. scikit-learn: For machine learning algorithms and preprocessing.
4. matplotlib: For plotting and visualization.
5. seaborn: For statistical data visualization.
6. mlxtend: For additional machine learning utilities and plotting.
7. statsmodels: For statistical modeling and graphics.
8. yellowbrick: For statistical visualization

# Note: if you have any problem with can not find dataset, then try to remove the folder_name in path <folder_name>/<file_name> => <file_name>

### 1. `prediction.py`

This script is used for predicting house prices using the Random Forest Regressor.

#### Steps to Use:

# Note: Please ensure that when you run the command, your path is in the correct directory. If not, use command cd <folder_name> to direct to the right folder.

1. **Load the Data**: Ensure that the dataset `Clean_dataset.csv` is in the correct path as the command.

2. **Run the Script**: Execute the script using the command:

   python prediction.py

3. Input Data: The script will prompt you to enter various features of the house such as CBD Distance, number of Bedrooms, Bathrooms, Car Garages, Landsize, Building Area, Property Age, and Suburb Name.

4. View Prediction: The script will output the predicted price of the house.

### 2. `Random_forest.py`

This script is used for predicting property sale potential using the Random Forest Classifier.

#### Steps to Use:

1. **Load the Data**: Ensure that the dataset `Reformatted.csv` is in the correct path as the command.

2. **Run the Script**: Execute the script using the command:

   ```sh
   python Random_Forest.py

   ```

3. Input Data: The script will prompt you to enter various features of the house such as Price, CBD distance, bedroom, bathroom, car garage, land size, re agency, median price and median rental.

4. View Prediction: The script will output "Sold" - S or "Not Sold" - NS

### 3. `KMeans.ipynb`

#### Steps to Use:

1. **Load the Data**: Ensure that the dataset `Clean_dataset.csv` is in the correct path as the command.

2. **Run the Script**: Open editor or complier which support jupyter notebook and run all the code.

3. Input Data: The script will prompt you to enter various features of the house such as CBD Distance, Landsize, Building Area as the second features beside the Prices.

4. View Prediction: The Final clusterd plot will show as output and the evaluation metrics will also be show.
