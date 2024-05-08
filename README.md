

<p align = "center"> 

  ![5-Sales-Tips-to-Increase-Conversion-and-Accelerate-Revenue](https://github.com/coding-dojo-data-science/Project1_Exemplar/assets/158508098/fa6f1995-6ae4-4cb4-b9fc-eb62849322d2)

</p>


# Prediction of Product Sales


Muhanned Shaheen

### The project will focus on sales prediction for food items sold at various stores. The goal is to assist the retailer in understanding the properties of products and outlets that play crucial roles in increasing sales

## Data Source: 
Big Mart Sales Prediction:
[https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/)

For this dataset, there were 8523 rows and 12 columns.

## Data Dictionary

<p align = "center"> 
  
  ![image_2024-05-04_151552633](https://github.com/MuhannedSh/Prediction-of-Product-Sales/assets/158508098/225eb62b-9322-4e36-9bf3-bc8691dbbcda)

</p>


## To prepare this data, the data was cleaned, and the following processes were performed:

### Exploratory Data Analysis
    - During the exploratory data analysis, a boxplot and histogram was visualized for numeric datatype. 
    - Also, a barplot and countplot was visualized for categorical column. 
    - This gave a good baseline for all of the numeric and categorical columns for univariate EDA.
    

<p align = "center"> 
  
  ![download (15)](https://github.com/MuhannedSh/Prediction-of-Product-Sales/assets/158508098/069f1321-203f-478a-9d9c-e38440117c3a)

</p>



- The histogram graph illustrates the frequency distribution of outlet item sales showing how many items fall into different sales value ranges, where the majority are around  $2000

<p align = "center"> 
  
  ![download (22)](https://github.com/MuhannedSh/Prediction-of-Product-Sales/assets/158508098/b278d6f7-65de-439b-a893-3e55fb6f9c24)


</p>

- The Figure illstrate that the highest counts are found in "Fruits and Vegetables" with 1232 instances, followed by "Snack Foods" at 1200 and "Household" at 910. Conversely, the lowest counts are seen in "Seafood" with 64 instances, "Breakfast" with 110, and "Starchy Foods" with 148. This distribution offers insights into the varying popularity of different item types within the dataset, informing strategic decisions regarding inventory management and marketing efforts.

 ### Expanatory Data Analysis 
    - To visualize the data for explantory purposes, three bargraphs were chosen and one linegraph was chosen.
    - The bargraphs were chosen to show how the categories compare to each other. 
    - Finally, a linegraph was chosen to show the trend of salaries over the past three years. 


## Explanatory Visuals

<p align = "center"> 

  ![download (16)](https://github.com/MuhannedSh/Prediction-of-Product-Sales/assets/158508098/fd3bfb68-8a37-4f3d-bf8e-3726f939b291)

</p>

- The Chart shows that the Greater than 0.20 of total display area of products, the lower item outler sale price profit.


<p align = "center"> 

![download (17)](https://github.com/MuhannedSh/Prediction-of-Product-Sales/assets/158508098/eb0f33e7-3d51-4cc8-9bea-69e7a243aff7)


</p>

- The Chart shows that there is a positive correlation between the maximum retail price and the target (r=0.57) , where the Greater MRP, the higher item outler sale price profit.


<p align = "center"> 

![download (18)](https://github.com/MuhannedSh/Prediction-of-Product-Sales/assets/158508098/d4d67311-ba3b-46ad-a87f-ad9608400f1a)



</p>

- the figure illustrate the outlet type to affect the outlet sales value
 

 ### Maching Learning Using the Following Models:
    - Bagged Tree Regressor Model
    - Tuned Bagged Tree Regressor Model
    - Random Forest Regressor Model
    - Tuned Random Forest Regressor Model
    
    
## Models Evaluated & Results

- Bagged Tree Regressor Model (Testing Set):
  - R^2: 0.54
  - MAE: 785.06
  - MSE: 1,282,522.17
  - RMSE: 1,132.48

  
- Tuned Bagged Tree Regressor Model (Testing Set):
  - R^2: 0.571
  - MAE: 764.818
  - MSE: 1,182,277.829
  - RMSE: 1,087.326


- Random Forest Regressor Model (Testing Set):
  - R^2: 0.562
  - MAE: 765.501
  - MSE: 1,209,445.919
  - RMSE: 1,099.748

- Tuned Random Forest Regressor Model (Testing Set):
  - R^2: 0.593
  - MAE: 745.291
  - MSE: 1,122,875.190
  - RMSE: 1,059.658




- The Final Model Chosen was a ` Tuned Random Forest Regressor Model`.
- For the testing set on the model, `59.3%` of the variance in y was explained by x. 
- The Mean Absolute Error was off by about `$745.29`.
- The Mean Squared Error was `$$1,122,875.19`.
- The Root Mean Squared Error had a calculation of `$1,059.66`.



Using this model to make sales predictions for food items sold at various stores would not be very reliable. The disparity between the R^2 score and the Root Mean Squared Error from previous regression metrics cannot be ignored


## Feature Importance - Using Tree Based Model

![download (23)](https://github.com/MuhannedSh/Prediction-of-Product-Sales/assets/158508098/1ff2cf19-0f73-4991-a6ac-aa937c09d6bd)


- Item_MRP (Item Maximum Retail Price): With a coefficient of 0.441817, Item MRP has the highest importance in predicting sales. This indicates that the maximum retail price of an item has a significant positive effect on sales. Specifically, for every unit increase in the maximum retail price, sales are expected to increase by approximately 0.44 units, holding all other variables constant.
  
- Outlet_Type_Grocery Store: With an importance coefficient of 0.191730, the type of outlet being a grocery store is the second most important feature. This suggests that the type of outlet significantly affects sales, with grocery stores having a notable impact compared to other types of outlets.
  
- Item_Visibility: Item visibility, with an importance coefficient of 0.099256, is the third most important feature in predicting sales. This implies that the visibility of an item within the store plays a moderately important role in driving sales. Specifically, higher visibility tends to lead to higher sales.

