# Bike Sharing: Multiple Linear Regression
> This project aimed to predict the demand for shared bikes in the American market post the Covid-19 lockdown for BoomBikes, a bike-sharing provider. The project began with comprehensive data preprocessing, including cleaning and encoding categorical variables. The dataset was split into training and test sets, and a multiple linear regression model was built, incorporating min-max normalization and feature selection using Recursive Feature Elimination (RFE). The model underwent meticulous refinement, considering VIF and p-values, resulting in a robust final model with an impressive R-squared score of 0.834 and an adjusted R-squared of 0.83 for the training dataset. The assumptions of linear regression were thoroughly validated, ensuring the model's reliability. The exploratory data analysis provided valuable insights into the impact of various categorical variables on bike demand. In conclusion, the project equipped BoomBikes with a powerful tool to understand and predict bike demand, enabling strategic decision-making in a competitive market.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)



## General Information
- This project aimed to predict bike demand for BoomBikes. Through thorough data preprocessing, feature engineering, and model refinement, the project successfully delivered a robust multiple linear regression model.
- BoomBikes, a bike-sharing provider, sought to understand the factors influencing the demand for shared bikes in the American market post-Covid-19 lockdown. The objective was to build a multiple linear regression model for accurate demand prediction, aiding BoomBikes in optimizing its business strategy.
- What is the business probem that your project is trying to solve?
- The dataset contains information on daily bike demands across the American market, considering various factors such as weather, season, year, temperature, etc. The target variable is 'cnt,' representing the total number of bike rentals, including both casual and registered users.



## Conclusions
- Univariate Analysis of Numerical Variables:
   - Temperature (temp) ranges from 2.4 to 35.3 Celsius, with a peak count between 10 to 15 Celsius.
   - Humidity (hum) spans from 0 to 97.2, with the highest count between 50 to 60.
   - Windspeed (windspeed) varies from 1.5 to 34, peaking between 8 to 13.
   - Bike demand (cnt) ranges from 22 to 8714, with the highest count between 4000 and 5000.
- Univariate Analysis of Categorical Variables:
   - Season 'fall' has the highest bookings, followed by summer, winter, and spring.
   - The year 2019 recorded more bookings than 2018.
   - Months from April to October have higher bookings, peaking in June and September.
   - Bookings are higher on non-holidays.
   - Weekdays show consistent bookings, with slightly fewer on Sundays.
   - Working days receive slightly more bookings than non-working days.
   - The majority of bookings occur in fair weather, followed by moderate and unfavourable conditions.
- Multivariate Analysis - Correlation:
   - Features 'temp' and 'atemp' positively correlate the most with 'cnt'.
   - 'yr' also positively correlates with 'cnt'.
   - 'Spring' and 'Jan' show a negative correlation with 'cnt'.
   - 'Sat' and 'Sun' negatively correlate with 'workingday'.
   - 'Hum' negatively correlates with 'fair_weathr'.
- Model Building (6th Model - Final):
Top Predictors:
   - Temperature (temp): Increases bookings by 0.4799 units.
   - Year (yr): Increases bookings by 0.2343 units.
   - Unfavorable Weather: Decreases bookings by 0.2062 units.


## Recommendations:
  - Focus on warmer locations for business expansion.
  - Avoid locations with unfavorable weather conditions.
  - Consider factors like windspeed, winter, Sep, fair_weathr, summer, and spring for boosting bookings.

  - Key predictors are temperature, year, and weather conditions.
  - Tailor marketing and business strategies accordingly.
  - Boost customer care during peak booking months.
  - Invest strategically in locations based on climatic and seasonal factors.




## Technologies Used
- pandas - version 2.1.2
- numpy - version 1.26.1
- seaborn - version 0.13.0
- matplotlib - version 3.8.2
- sklearn - version 1.3.2
- statsmodels - version 0.14.0


## Acknowledgements
- would like to thank UpGrad for giving us the oppurtunity to work on this project. 


## Contact
Created by [Imliyangla](https://github.com/Imliyangla) - feel free to contact me!


