# Project 2: Project 2 - Ames Housing Data and Kaggle Challenge
## General Assembly DSI-9-ATL
## James Proctor

### **Problem Statement:**
Zillow will often indicate "Estimated home price" to inform users about the market rates of homes, even when they are not yet explicitly for sale. More accurate depictions of home values translates to more confidence in Zillow's product, and will therefore grow their user base (translating to more advertising revenue).

Given data on sold residential properties in Ames, Iowa, I was tasked with cleaning and interpreting the given features of the data and creating a linear regression model to predict the sale price.

Next, my models were tested on a separate dataset that did not include the sale price of the data. I used my model to predict the sale price of the new data using the same laboriously constructed set of features on which I built my model.

Models were scored based on the true sale price by calculating Root Mean Squared Error.

The project culminated in a formal, semi-technical presentation.

### Executive Summary:

##### Contents:

- Package Import
- Data Import and Cleaning
- Data Familiarization and Cleaning
  - Looking for missing values
  - Replacing null values
  - Transforming Nominal Data to Ordinal
  - Checking correlation for feature engineering.
- Exploratory Data Analysis
  - Log Transformation
  - Feature Building
  - Feature Interactions
  - Visualizing Categorical Variables
  - One Hot Encoding: Dummy Variables
  - More Interaction Features
- Final Clean Dataframe to CSV
- Feature Selection
  - Tracking Model Performance
- MODELING
  - Variable Construction
  - Train Test Split
  - Data Scaling
 - Ridge
 - Lasso
 - Elastic Net
 - Linear Regression
- Kaggle Submission


### The Data:
The provided data set included property characteristics for 2050 sold properties in Ames, Iowa. All properties in the data were sold from 2006-2008.

The characteristics included typical property features (eg. number of bedrooms and bathrooms; square footage), as well as ratings for house quality or condition, construction materials, zoning data, and location data.

More in depth description of the data can be found _[here.](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)_

### Conclusions:

My final model selection was a Multiple Linear Regression Model that incorporated 64 features. I engineered many of these features with Polynomial and Cubic Interactions, along with one-hot encoding for many of the nominal features (eg. neighborhood) and some of the ordinal features (eg. total bathroom number). Of the 50+ dummy variables that I created, I only used the one that correlated with the target variable (log-saleprice) > 0.2 or <-0.15.

I found that the model performance between different regularization techniques was negligible, but I settled with Ridge because it gave me the best score on Kaggle. It was interesting to see the ways in which different regularization techniques treated the many included features, and how the models performed near equivalently despite some variable coefficients being reduced to zero by Lasso and Elastic Net.

### Main Takeaways and Future Improvements:
 - Improve Feature Engineering and Selection:
   - Recursive Feature Selection
   - Reduce Multicollinearity
- Find better ways to interact quality and square footage.
- Convert 'quality' to a more understandable metric (eg. cost for improvements).
- Impute missing data more effectively:
  - Zeroing missing numeric data reduces predictive power of the variables.
- Collect More Data:
  - Incorporate interactions with buyers and sellers
  - (eg. Listing vs Final Sale Price)
