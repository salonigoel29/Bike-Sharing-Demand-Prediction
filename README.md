# Bike Sharing in Washington DC
### About the project
Rental bikes in 2011 and 2012 with corresponding weather and seasonal information. 
The goal is to forecast bike rental demand of Bike sharing program in Washington, D.C based on historical usage patterns in relation with weather, time and other data.
Using these Bike Sharing systems, people rent a bike from one location and return it to a different or same place on need basis. People can rent a bike through membership (mostly regular users) or on demand basis (mostly casual users). This process is controlled by a network of automated kiosk across the city.


### About the Data Set
The dataset shows hourly rental data for two years (2011 and 2012). The training data set is for the first 19 days of each month. The test dataset is from 20th day to month’s end. We are required to predict the total count of bikes rented during each hour covered by the test set.
In the training data set, they have separately given bike demand by registered, casual users and sum of both is given as count.
Training data set has 12 variables (see below) and Test has 9 (excluding registered, casual and count).

#### Data Dictionary :
1. datetime: Date
2. season: Season (1:spring, 2:summer, 3:fall, 4:winter)
3. holiday: weather day is holiday or not (extracted from Holiday Schedule)
4. workingday: If day is neither weekend nor holiday is 1, otherwise is 0.
5. weather: (extracted from Freemeteo)
        1: Clear, Few clouds, Partly cloudy, Partly cloudy
        2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
        3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
        4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
6. temp: Normalized temperature in Celsius. The values are derived via (t-tmin)/(tmax-tmin), tmin=-8, t_max=+39 (only in hourly scale)
7. atemp: Normalized feeling temperature in Celsius. The values are derived via (t-tmin)/(tmax-tmin), tmin=-16, t_max=+50 (only in hourly scale)
8. humidity: Normalized humidity. The values are divided to 100 (max)
9. windspeed: Normalized wind speed. The values are divided to 67 (max)
10. casual: count of casual users
11. registered: count of registered users
12. cnt: count of total rental bikes including both casual and registered
