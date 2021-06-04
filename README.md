# Kings-County-Housing-Predictions

This project conducts an analysis on the housing prices of Kings County, Seattle. From the data given of each house, a linear regression model was created to predict the prices of the houses. Location, living space and condition of the house were some of the attributes to consider when creating the model. 

# Column Names and descriptions for Kings County Data Set
* **id** - unique ID for a house
* **date** - Date day house was sold
* **price** - Price is prediction target
* **bedrooms** - Number of bedrooms
* **bathrooms** - Number of bathrooms
* **sqft_living** - square footage of the home
* **sqft_lot** - square footage of the lot
* **floors** - Total floors (levels) in house
* **waterfront** - Whether house has a view to a waterfront
* **view** - Number of times house has been viewed
* **condition** - How good the condition is (overall)
* **grade** - overall grade given to the housing unit, based on King County grading system
* **sqft_above** - square footage of house (apart from basement)
* **sqft_basement** - square footage of the basement
* **yr_built** - Year when house was built
* **yr_renovated** - Year when house was renovated
* **zipcode** - zip code in which house is located
* **lat** - Latitude coordinate
* **long** - Longitude coordinate
* **sqft_living15** - The square footage of interior housing living space for the nearest 15 neighbors
* **sqft_lot15** - The square footage of the land lots of the nearest 15 neighbors

# Creating the Model
1. Exploratory data analysis was done on the data. There were some outliers and extreme values eg. 33 bedrooms in one house. Sqft_living had the highest correlation with price
2. Data was cleaned by getting rid of those outliers. 
3. Some statistical tests were ran to check the significance of variables to the price of the house. 
4. A few new features were manually engineered to make the model predict better. 
5. A linear regression model was ran using the train_test method. Our target variable was price. 
6. Other models were created using the feature selection methods such as polynomial, K-best and Recursive feature elimination.
7. Using pickle the model was imported to another file and tested on a test data set to predict the prices. 

# Files in the Repo
1. In the data folder there are 3 files, one for data to test the model on named kc_house_data_test_features, one for data the model was made on, named kc_house_data_train and the third is the one that has predictions of the prices.
2. The pickle folder has 2 files, one has the model in it and the second has the features of the model. 
3. The 2 notebooks are, one has the EDA, feature engineering and model creating process called Kings County and the other has the model predicting the on the data called predict_holdout. 
