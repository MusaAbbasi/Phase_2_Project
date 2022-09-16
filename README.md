# Phase_2_Project
 
Kings County House Price Project
An analysis of house price data in Kings County, Washington

Overview
This is project in which we analzyed house prices in Kings County Washington based on infromation provided of houses sold in the county in 2014.  For this assignment, we simulated our stakeholder as being a real estate agency looking to figire out what were the most important criteria for determining a house's price. We created a regression model that would provide the best way to determine a house's price, and determined which criteria, based on the information we found and the EDA we did on the data we had, were the best predictors of house price. Ater doing the EDA, we decided the best way to do this was to create a simple regression model based on using all variables in the data provided. The next step was adding in additional information about zipcode data for each house sold that was in our data, and removing variables and wrangling the data to create a more optimized model. After testing different models, we created our final model, which was 81% accurate in predicitng house prices based on the criteria we selected. Based on this, we determined qualities such as square foot living area, number of bathrooms, if a property was on the waterfront, or if it had a basement, were the most important variables in determing house price, as well as zip code, a proxy for nwighborhood, which was the variable that had the most effect on determining house price,

Business Understanding
A real estate agency wants to know the most important criteria for determing house price in Kings County, Wahington. 

Data Understanding and Analysis
Our data came from a dataframe of information regarding roughly 21,000 houses sold in Kings County, Washington in the year 2014. We also used information about the zipcodes, cities, and population for each city from a separate data frame, which we merged with our original data. After cleaning the data, we had infromation on approximately 15,000 houses in Kings County. 

Our initial model based on this cleaned data only had a R squared value of 0.58. After playing arounf with the data, and removing any outliers, we created a model with 61% accuracy. At this stage, we decided we needed more information to make our model better, which is where we added information about zipcodes. The model created after this had a R squared value of 0.792, a signigicant improvement. However, we noticed that the model was more accurate at predicitng relatively cheaper homes, and was more inaccurate the more expensive a house was. Recognizing this, we ran our models again with a dataset in which houses worth over $2 mmillion were removed. As this is a very high threshold, we only lost roughly 150 datapoints, and still had data on 14960 houses. This final model, after some more adjusting of variables, had an R-squared value of 0.818. After training the model, the R-squared of the test set was 0.817.

Description of Data


Conclusion
The most important criteria for determining house price in Kings County, according to the data we collected, was zip code. While not something that was found in our data, we are assuming the reason for this is that zipcodes are numbers that designate relatively small areas in which house prices might be similar, making zipcodes, in this model, proxies for neighborhoods. We found that after this, the best predictor variables for predicting house prices were the square footage of the living area of the house, not necessarily the whole area of the property, the number of bathrooms, if a house was on the waterfront, and finally, if a house had a basement.
