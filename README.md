# Predictive Analysis of Sales Data:
Dataset used: https://www.kaggle.com/datasets/shivan118/big-mart-sales-prediction-datasets/data
# About Dataset
## Sales Prediction for Big Mart Outlets
The data scientists at BigMart have collected 2013 sales data for 1559 products across 10 stores in different cities. Also, certain attributes of each product and store have been defined. The aim is to build a predictive model and predict the sales of each product at a particular outlet.

Using this model, BigMart will try to understand the properties of products and outlets which play a key role in increasing sales.

Please note that the data may have missing values as some stores might not report all the data due to technical glitches. Hence, it will be required to treat them accordingly.

## Data Dictionary
We have a train (8523) and test (5681) data set, the train data set has both input and output variable(s). You need to predict the sales for the test data set.

### Train file:
CSV containing the item outlet information with a sales value

**Variable Description :** 
* **Item_Identifier** : Unique product ID
* **Item_Weight** : Weight of product
* **Item_Fat_Content** :  Whether the product is low fat or not
* **Item_Visibility** : The % of the total display area of all products in a store allocated to the particular product
* **Item_Type** : The category to which the product belongs
* **Item_MRP** : Maximum Retail Price (list price) of the product
* **Outlet_Identifier** : Unique store ID
* **Outlet_Establishment_Year** : The year in which the store was established
* **Outlet_Size** : The size of the store in terms of ground area covered
* **Outlet_Location_Type** : The type of city in which the store is located
* **Outlet_Type** : Whether the outlet is just a grocery store or some sort of supermarket
* **Item_Outlet_Sales** : sales of the product in t particular store. This is the outcome variable to be predicted.

### Test file:
CSV containing item outlet combinations for which sales need to be forecasted

**Variable Description :** 
* **Item_Identifier** : Unique product ID
* **Item_Weight** : Weight of product
* **Item_Fat_Content** :  Whether the product is low fat or not
* **Item_Visibility** : The % of the total display area of all products in a store allocated to the particular product
* **Item_Type** : The category to which the product belongs
* **Item_MRP** : Maximum Retail Price (list price) of the product
* **Outlet_Identifier** : Unique store ID
* **Outlet_Establishment_Year** : The year in which the store was established
* **Outlet_Size** : The size of the store in terms of ground area covered
* **Outlet_Location_Type** : The type of city in which the store is located
* **Outlet_Type** : Whether the outlet is just a grocery store or some sort of supermarket
---
  ### Libraries to be installed :
  * **pip install numpy**
  * **pip install pandas**
  * **pip install matplotlib**
  * **pip install seaborn**
  * **pip install scikit-learn**
 ### Regression Model:
I have use Random Forest model for this Regression Model because its gives the best prediction With a accuracy of 56.45%.<br>
<br>**About Random Forest Model :**
* **Ensemble Learning:** Random Forest combines multiple decision trees for regression tasks.
* **Reduced Overfitting:** It uses random subsets of features and data, reducing overfitting.
* **Bagging:** Multiple trees are trained on bootstrapped samples of the data.
* **Feature Importance:** It provides a measure of feature importance for feature selection.
* **Robustness:** Less prone to overfitting compared to individual decision trees.
* **Missing Values Handling:** Can handle missing data without needing imputation.
* **Non-linear Relationships:** Effective at capturing non-linear relationships in data.
* **Parallelization:** Easily parallelized for efficient training on multicore processors.
* **Out-of-Bag Error:** Estimates model performance without requiring a separate validation set.
* **Versatility:** Suitable for various regression tasks across different domains.
