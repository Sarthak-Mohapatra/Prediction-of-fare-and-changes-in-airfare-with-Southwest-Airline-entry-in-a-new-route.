# Airfare prediction with SouthWest Airlines entry in a new route.
Predicting the airfares and changes in airfares with SouthWest Airlines entry in a new route. The key question what I have tried to answer 
is: Whether the presence or absence of Southwest Airlines (a low-cost entrant) would have any effect on fare?


## Table of Contents

* General Info
* Variable Description
* Screenshots
* Technologies and Tools
* States
* Contact

## General Info

The data set contains the real data that were collected between Q3-1996 and Q2-1997. Data Cleanup was done initially to ensure that
there are no NULL records in the dataset. After ensuring proper data in the data set, Exploratory Data Analysis was done to understand 
the data distribution and the correlation between variables. Linear Regression with subset selection process was used on the data set to
predict the air fares.

## Variable Description

The data set contains 18 variables. The variable names and the description is mentioned below:
  - S_CODE:   Starting airport’s code
  - S_CITY:   Starting city
  - E_CODE:   Ending airport’s code
  - E_CITY:   Ending city
  - COUPON:   Average number of coupons for the route
  - NEW:      Number of new carriers entering that route between Q3-96 and Q2-97
  - VACATION: Whether (Yes) or not (No) a vacation route
  - SW:       Whether (Yes) or not (No) Southwest Airlines serves that route
  - HI:       Herfindahl index, a measure of market concentration (higher number means smaller number of available carriers on that route)
  - S_INCOME: Starting city’s average personal income
  - E_INCOME: Ending city’s average personal income
  - S_POP:    Starting city’s population
  - E_POP:    Ending city’s population
  - SLOT:     Whether or not either endpoint airport is slot-controlled
  - GATE:     Whether or not either endpoint airport has gate constraints
  - DISTANCE: Distance between two endpoint airports in miles
  - PAX:      Number of passengers on that route during period of data collection
  - FARE:     Average fare on that route
  
 ## Screenshots
 
 The below screenshot shows the correlation between variables. Few of the major observations are mentioned below:
 
 ![Heat Map shwoing correlation](https://github.com/Sarthak-Mohapatra/Prediction-of-fare-and-changes-in-airfare-with-Southwest-Airline-entry-in-a-new-route/blob/master/Heat%20Map.png)
 
* 1 - It can be seen that FARE has highest positive correlation with DISTANCE. 
It would mean that with increase in distance, the FARE is going to increase. 
* 2 - DISTANCE has a strong positive correlation between COUPON. 
It means that, if distance between two points is more, then it is likely that there will be more coupons for that route.
* 3 - DISTANCE has the high negative correlation with HI. 
It can mean that, if distance between two points is less, then there would be lesser flights opertaing and so the HI index would be more.**
* 4 - COUPON has the highest positive correlation with DISTANCE. 
It would mean that if distance is more, then there is a possibility that there will be more coupons for that route.
* 5 - COUPON has high negative correlation with HI. 
It would mean that if a route has lesser flights, then the HI index would be more and coupons for that route will be less.


## Technologies and Methods

* R-Studios
* Microsoft Excel
* Linear Reression
* Subset Selection Process (Regsubsets and StepAIC)

## Status

Project is: *finished*

## Contact

If you loved what you read here and feel like we can collaborate to produce some exciting stuff, or if you just want to shoot a question,
please feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/sarthakmohapatra1990/).

