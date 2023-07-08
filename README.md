# Project Name
> Telecom Churn Prediction


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information

**Overview**
Telecom Industry is a very competitive market, exit barriers for customer are low. Loyalty depends on user experince and attractive offers. Industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition. Retaining high profitable customers is the number one business goal.
 

**Problem Statement**
To reduce customer churn, telecom companies need to predict which customers are at high risk of churn. 
- The goal is to build a predictive model that can predict the chrun propensity for a customer accurately.
- Identify key features that indicates the customer behaviour to churn

**Approach**

STEP 1 : Data Understanding, Preparation, and Pre-Processing :
Data understanding, identification of potentially useful and non-useful attributes and variable importance and impact estimation Data preparation, performing data cleaning, missing values imputation, outlier removal, and column level standardization (for e.g., date, etc.) into one format

STEP 2 : Exploratory Data Analysis :
Performing basic preliminary data analysis including finding the correlation between variables and scatter plots to identify relationships between variables Performing advanced data analysis, including plotting relevant heatmaps, histograms, and basic clustering to find patterns in the data

STEP 3 : Feature Engineering and Variable Transformation :
Feature engineering and performing one or more methods on attributes that can lead to the creation of a new potentially useful variable; for e.g., day from the date Variable transformation and applying categorical variable transformations to turn into numerical data and numerical variable transformations to scale data

STEP 4 : Model Selection, Model Building, and Prediction :
Identifying the type of problem and making a list of decisive models from all available choices Choosing a training mechanism; for e.g., cross-validation, etc., and tuning hyperparameters of each model Testing each model on the respective model evaluation metric Choosing the best model based on the fit of the data set and output variable Using ensemble options to improve the efficacy based on the evaluation metric stated in the problem

STEP 5 : Business Recommendation


## Conclusions
- Our primary aim is to reduce customer churn, so it becomes utmost important to identify potential churning customers
- Given this scenario, the most important metric will be SENSITIVITY
- Logistic Regression with feature selection using Random Forest and RFE becomes the best model from business perspective
- This model has
	- accuracy = 0.77 (77% of the predictions are correct)
	- sensitivity = 0.84 (84% of the customers who are churning can be identified)

- Most important features are -

	- 'arpu_6',
	- 'arpu_7',
	- 'arpu_8',
	- 'roam_og_mou_8',
	- 'loc_og_mou_8',
	- 'loc_ic_t2t_mou_8',
	- 'loc_ic_t2m_mou_8',
	- 'loc_ic_mou_7',
	- 'std_ic_t2m_mou_8',
	- 'total_rech_num_8',
	- 'max_rech_amt_8',
	- 'last_day_rch_amt_8',
	- 'aon',
	- 'rchrge1_no_of_days'

**Recommendations**
- Average revenue per user (arpu) shows a constant decline from June to August for churning customers. So, sales team may talk to customers who are showing this decreasing trend and may provide discounts and offers as per their need.
- roam_og_mou_8 is an important predictor variable looks like customers are churning for better roaming plans. Business can come up with better roaming packs for it's customers
- There is a decrease in incoming and outgoing calls usage for churning customers. If business finds a decrease in the mou then they should try to retain those customers by coming up with better offers, most likely unlimited plans etc. This may be also due to poor network service in some area. In this case, network needs to be improved in that area
- Same trend is observed with recharge columns. A decrease in average recharge amount or increase in number of days since last recharge is an indicator of churn. Provide offers and discounts
- Age on network 'aon' is also an important feature. Old customers are least likely to churn. However, relatively new customers are most likely to churn. Sales team must provide some offers to new high revenue customers, so that they do not churn

## Technologies Used
- pandas library - version 1.3.5
- numpy library - version 1.20.1
- matplotlib library - version 3.3.4
- seaborn library - version 0.11.1
- statsmodels - version 0.12.2
- sklearn - version 0.24.1
    - sklearn.linear_model
    - sklearn.preprocessing
    - sklearn.model_selection
    - sklearn.feature_selection
    - sklearn.metrics
    - sklearn.decomposition
    - sklearn.ensemble
    - sklearn.tree
    - sklearn.inspection
- datetime
- xgboost



## Acknowledgements
- This project was based on Machine Learning ML2 Module for the Executive PG Programme in Machine Learning & AI - IIIT,Bangalore.


## Contributors
- <a href="https://github.com/pradeepksharma22/">Pradeep Kumar Sharma</a>


