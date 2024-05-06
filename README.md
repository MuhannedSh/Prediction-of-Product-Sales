

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




- The Final Model Chosen was a `Random Forest Regressor Model` with the n_estimators tuned to 50.
- For the testing set on the model, `56.2%` of the variance in y was explained by x. 
- The Mean Absolute Error was off by about `$765.50`.
- The Mean Squared Error was `$1,209,445.92`.
- The Root Mean Squared Error had a calculation of `$1,099.75`.

Using this model to make sales predictions for food items sold at various stores would not be a very reliable. Considering the previous regression metrics from how the model performed, there is a disparity between the R^2 score and also the Root Mean Squared Error that cannot be ignored.

## Recommendations

Data Science Insights

- For those who have an interest in Data Science:
  - Data Analytics Leads & Principal Data Engineers earn the most amount of money. However, this are usually not entry level careers and I would recommend going through a program, like Coding Dojo, where you can earn your data science certificate and then map out your career to these positions.

  - Data Engineers & Data Scientists have the most 100% remote positions. So, if you are wanting to work from home, or work from anywhere in the world, choosing one of the top five remote positions would be a good choice to build your career upon.
  
  - Lastly, the trend for the last three years show that data science and related fields are increasingly earning more money each year. So, choosing a career in one of these fields can be very lucrative.

Model Performance
- Overall, the best model is definitely the tuned Random Forest Regressor Model. There was still some bias in the model, but by far it outperformed the linear regression model. 


## Limitations & Next Steps

From here, a student could use the insights from the visuals on how to tailor their path for their career. As mentioned before, Coding Dojo has a fantastic program that prepares inspiring data scientists for the field of data science. 

## For Further Information

For any additional questions, please contact: 
- Sherlin Whaley (Data Science Instructor)
- swhaley@codingdojo.com

