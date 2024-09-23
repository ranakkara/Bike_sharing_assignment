# Bike sharing assignment - Multiple Linear Regression 
> A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)



## General Information
### Objective
Build a model and find variables significant for the demand of shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

To achieve this following are the activities carried of
- Understanding and Reading dataset
- Data cleaning
- Exploratory data analysis
- Data preperation
- Model Building
- Making Predictions Using the Final Model on Test set
- Model Evaluation


## Conclusions
### Significant variables
1. **Temperature**
    - Coefficient : 4996.876
    - Significance : Highly significant (p-value < 0.0001).
    - interpretation : Higher temperatures lead to increase in bike demand.
2. **Season**
    - Summer
        - Coefficient : 710.791
        - Significant : Highly significant (p-value < 0.0001).
    - Winter
        - Coefficient : 1210.971
        - Significant : Highly significant (p-value < 0.0001).
    - interpretation : Demand is higher during Summer and winter season.
3. **Year**
    - Coefficient : 2014.304
    - Significance : Highly significant (p-value < 0.0001).
    - interpretation : There is a growing demand on bikes year on year.
4. **Month**
    - Coefficient : 900.310
    - Significance : Highly significant (p-value < 0.0001).
    - interpretation : Demand is higher in September month.
5. **Weekday**
    - Coefficient : 569.994
    - Significance : Highly significant (p-value < 0.0001).
    - interpretation : Demand is higher on Saturdays.
6. **Working-day**
    - Coefficient : 500.288
    - Significance : Highly significant (p-value < 0.0001).
    - interpretation : Demand is higher on working days.
7. **Weather Condition**
    - Good Weather
        - Coefficient : 2634.468
        - Significance : Highly significant (p-value < 0.0001).
    - Moderate weather
        - Coefficient : 2634.468
        - Significance : Highly significant (p-value < 0.0001).
    - Interpretation : Better weather conditions significantly increase bike demand
### How well Significant variables describe the bike demand
1. **R-squared Value :**
    - R-squared value of test data which is 0.800 is very close to the train data which is 0.823, which means the R-squared values for the training and test data are quite close (0.823 for training and 0.800 for testing). This consistency suggests that the model performs similarly on both the training set and the unseen test set.This indicates that approximately 80% to 82% of the variance in bike demand can be explained by the variables included in the model. This suggests a strong fit.

2. **Statistical Significance :**
    - All significant variables (with p-values < 0.05) reinforce that they are likely to have a real effect on bike-sharing demand.
3. **Model Adequacy:**
    - The adjusted R-squared value accounts for the number of predictors in the model, indicating that the model maintains a good explanatory power even when considering model complexity.

### Recommendations for high Profits
1. `Summer Campaigns:` Implement targeted marketing campaigns during the summer and winter months to capitalize on higher demand.
2. `Weather-Based Promotions:` Offer discounts or promotions on days with favorable weather conditions to attract more users.
3. `Targeted Marketing:` Focus on increasing awareness and accessibility in urban areas where temperatures are likely to rise and where biking is a feasible commuting option.
4. `Enhance User Experience:` Improve bike availability and maintenance during peak seasons, particularly in good weather, to ensure customer satisfaction and repeat usage.
5. `Community Engagement:` Partner with local events, especially during weekends, to provide bike rentals, which can increase visibility and usage.

## Technologies Used
- Python - 3.12.4
- NumPy version - 1.26.4
- pandas version - 2.2.2
- Matplotlib version - 3.8.4
- Seaborn version - 0.13.2
- sklearn version - 1.4.2
- statsmodels version - 0.14.2
