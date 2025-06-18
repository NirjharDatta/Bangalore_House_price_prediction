# Bangalore_House_price_prediction
In this project, I have tried fitting a regression model to the Bangalore house price dataset. This is my first AI project and feeling very excited to share.
# Dataset
[Banagalore_house_price.csv](https://github.com/user-attachments/files/20775813/Banagalore_house_price.csv)
-This dataset contains the price of Bangalore house prices and various categorical and numerical features.
# Features Used
  | Feature Name | Data Type    | Description (Optional)                |
|--------------|--------------|----------------------------------------|
| area_type    | Categorical  | Type of area (e.g., Super Built-up, etc.) |
| zone         | Categorical  | Geographic location of the property   |
| size         | Categorical  | Number of BHKs/Bedrooms               |
| availability | Categorical  | Ready to move/immediate possesion/date |
| total_sqft   | Numerical    | Total area in square feet            |
| bath         | Numerical    | Number of bathrooms                  |
| balcony      | Numerical    | Number of balconies                  |
| price        | Numerical    | Target variable (price in lakhs)     |
# Updated dataset for use:(self modified)
[updated_sheet.csv](https://github.com/user-attachments/files/20776137/updated_sheet.csv)
- This dataset contains the features after modification, ready for use in my ML model.
# Steps: 🚀
   * Correct data types of all data to integer or float for model.
   * Perform Coversion for data present in different units.
   * Remove or replace null data. (replace with best match, mean or delete)
   * One hot encoding of categorical data.
   * For categorical data if too many categories, reduce to lesser no. of categories
   * Calculate and replace with mean for range data.
   * Fit a regression model with features and different degrees.
   * Better performance with degree 3,4 on train data but overfitting with test data but best train and test fit with degree 2.
   * Regularize model with different alpha values. Better fit for alpha=1 in my model .
   * Changed scaling from standard scaler to robust scaler.
   * Changing each feature individually to have better correlation with price.
   * Remove outliers .Check non-binary feature separately.
   * Take log(1+x) for skewed features.
# Result: 🏆
Obtained a ML model with r2_score of 0.684 in training data, 0.662 in testing data and 0.6734 for the complete dataset.
