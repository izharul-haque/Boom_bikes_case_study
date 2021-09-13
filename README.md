# Boom_bikes_case_study
Creating model using Linear regression to predict variables impacting demand

![image](https://user-images.githubusercontent.com/76435558/133163816-8b88bae7-f72e-4e51-86b0-f94da5746ad6.png)

# Problem Statement
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain 
in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, 
and the economy restores to a healthy state.

### The company wants to know:
- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands.

# Business Objectives:
Required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different 
features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management 
to understand the demand dynamics of a new market.

# Dataset Description
The dataset provided contains all the information of the bike registered and casual users along with the other variables impactiong the daily rent.

# Climate Condition Vs Count of the Renters
![image](https://user-images.githubusercontent.com/76435558/133163965-28748c14-e543-4282-9c4a-3fc6aad2b5c5.png)

### From above plot we can state that during clear weather the numbers of riders renting the Bikes are more as compare to the Mist/Cloudy weather
- We can see that the riders use to access the services more during Mist/cloudy or Clear weather.
- During light snow/light rain and the user won't prefer to avail the services if it's non-working day but during working days they do have rented the bike a very few nos of times.
-
# Correlation among independenet variables

![image](https://user-images.githubusercontent.com/76435558/133164234-1f0c5026-9b12-477d-86e7-bf68085f4514.png)

### Inferences

- workingday variable has high negative correlation with Sat & Sun (where workingday =0)

- season_spring is highly negatively correlated with count and temp.

- temp and count has strong correlation.

- weathersit_cloudy and humidity has moderate correlation

#### We can see that temperature,Summer season,June to October months are in good correlation with the 'count' variable. And seem to have good influence on the number of bike rentals.

## Model build using 15 Featured Variables using Statsmodel for detail analysis and further optimization of the model.
### 11 models created and and finalized model 8 as final model
- p-Values for all variables are < 0.05 All values of VIF are < 5
- The number of variables are 10 excluding the constant which has given the desired R-squared, p value and VIF
- R-squared: 0.833
- Adj. R-Square: 0.830

# Model Evaluation

![image](https://user-images.githubusercontent.com/76435558/133165119-c2b05a7f-0803-4978-abc7-e21b100b5014.png)

- Hence, We reach to the decent model for the the demand for shared bikes with the significant variables
- R-Square: 83.3%
- Adj. R-Square: 83.0%
- F-Statistics: 249.2

# Important & Significant Features(predictors) which effect demeand for shared bikes:
- Temperature has a high coefficient of 0.4156, which means that if the temperature increases by 1 unit the demand goes up by 0.4156 units.
- During cloudy and light snow rain climate the demand for renting a shared bike goes down as these variables are negatively corealted with the negative coefficient of -0.2485 and -0.696 respectively.
- Similarly, During Summer and winter the user prefer to rent a bike so the provider can introduce some offer or increase the promotion to boost the sales and during spring the demand goes down and for boosting the sales the providers can introduce some small budget plan.
- Another Important point to infer that yearly demand is going up and the rental number is increasing by the positive coefficient of 0.2034
