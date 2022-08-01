# PyBer_Analysis


## Overview of Analysis:


The following analysis is done with using two csv's, city data and ride data. To create the line chart needed for this challange the first step was to load in the file from the two csv's used in this challange and then after loading in the data the data was merged to create a DataFrame to have the city, data, fare, ride_id, driver_count, and region type. Then after the merge the next dataframe needed was a summary dataframe and to create that there are 6 variable that are needed. Total rides, Total Drivers, Total Fares, Average Fare per Ride, Average Fare per Driver. To create these variable the df.groupby method was used and depending on what that variable was supposed to represent either .count(), .sum(), .mean() was used. The only different variable was the Average Fare by Driver was different since it ised total fares divided by total drivers to get the average. For deliverable 2 the variable used for the graph was .sum() for fare, and was group by the date, and type. And then a pivot table was created using fare for values, date was used for the index, and the type was used in the columns, and then was given a specif data from 1-1-2019, to 4-9-2019. After the date index was set to a datatime datatype so that the pivot table could be resampled to use week. After the resampling the line chart was created using the fivethrityeight style, with a figsize of (20 ,10).


## Results Analysis:


![dataframe_totals](https://user-images.githubusercontent.com/97326526/182220320-ed8e3b07-77dd-4518-ac33-1c7770f737ca.JPG)


# Rural:


The total rides for this type of region is lowest with 125 rides, since it will have the lowest population amount, also the lowest amount of drivers with only 78, due the low ride demand, so not much demand for drivers. Rural region type also had the lowest amount of total fares with $4,327.93 due to low ride demand. But the Rural region type has the highest average for per ride with $34.62 and highest average fare per driver with $55.49 compared to the other region types since the demand is low the fare will have to higher to keep drivers.


![rural_data](https://user-images.githubusercontent.com/97326526/182220965-e227aeff-544e-4ec9-acbe-ea925d966205.JPG)


# Suburban:

The suburban region type is the middle point of the three region types with a good amount more demand for rides. The total rides are 625 which is a 500 ride increase compared to rural, and the total driver also has an increase to 490 which is a 412 increase since there is more of a population compared to the rural area type. The total amount of fares has also quite a significant increase with a total fares being $19,356.33 which is a $15,028.40 increase of total fares. The average ride fare is lower than the rural due to higher demand for rides with $30.97 per ride which is only a $3.65 decrease per ride. And the average fare per driver is 39.50 which is decreased by 15.99 compared to rural driver fare.


![suburban_data](https://user-images.githubusercontent.com/97326526/182224736-1e463ec0-c12f-4d4d-8e05-efb611ce6040.JPG)


# Urban:


Urban is highest population density so it has the highest amount of total rides at 1,625 which is 1,000 more rides compared to suburban region, and has 2,405 total drivers which is a 1,915 more drivers than suburban, and is the first time that there are more drivers than we have rides. The total amount of fares is $39,854.38 which is a $20,498.05 increase to the suburban region. The average fare per ride has a significant decrease due to more demand for rides urban average per ride is $24.53 a decrease of $6.44. The average fare for the driver is $16.57 due to the commision taken from the driver and the high amount of drivers in the area making the average for the driver fare lower. The decrease is quite massive compared to suburban with a difference of $22.93. 


![urban_data](https://user-images.githubusercontent.com/97326526/182227769-9ef9fb68-8a55-4805-b91b-f14b247ea587.JPG)


## Summary

> - Recommendations:


1. The first recommendation to fix a major disparity in the urban regions average fare per driver is to not hire any new drivers in urban areas while there is an over saturation of drivers in the urban market causing the average fare for drivers to go down quite significantly. The only propblem is that there will need to be some sort of system put in place where drivers who drive more often are given more incentive to keep driving so not to have a shortage of drivers on the road to have high wait times for customers.


2. The second recommendation is to raise the Urban areas fares to increase the average for average drivers, this could be done to bypass the first recommendation is a easier solution to not only raise averages of fare per driver but to also increase fare per ride and total fare. The only con to this recommendation is that we may a competitor with better prices that the customers may go to but more drivers may be incetived to drive with us making us have lower wait times.


3. Third is if we raise prices to the Urban areas we may also want to raise the suburban fare prices to have a higher average fare per driver, but also to increase total fares to equilize with urban areas. The only problem is that in suburban area the competitor may have lower prices than us and wait times may already be pretty low in suburban area due to not that high of a ride demand. 
