# PyBer Rideshare Project Analysis

## Overview
We reviewed data for PyBer rides from 1/1/2019 through 5/8/2019 to identify trends. Data provided included a ride ID, the city the ride occurred in, the date the ride occurred, and the total fare for the ride. We also had data that classified each city as urban, suburban or rural, and listed the count of PyBer drivers working in that city. 

In looking to identify differences in performance between markets (urban, suburban or rural) we summarized data based on city type into these three categories, identified the 5 key metrics as total rides, total drivers, total fares, average fare per ride and average fare per driver. 

We also plotted total fare by week, for January through April, by city type, in order to see if there were any peaks or dips at different points in the timeframe, and if those were consistent or differed between city types. 

## Results

### Assumptions about the three city environments

Prior to detailing comparisons in the key metrics, we would like to review some key assumptions about each type of city that impact those results and our interpretation of them.
1. **Rural** We would expect cities classified as rural to exhibit the lowest population density, and due to being more spread out, the highest percentage of personal vehicle ownership. There is little in the way of events and nightlife where a PyBer ride may be desired even amongst those with their own vehicle. Most businesses will have ample parking, so lack or cost of parking is unlikely to be a concern. 
2. **Urban** We would expect cities classified as urban to exhibit the highest population density, and due to being more compact with parking at a premium, the lowest percentage of personal vehicle ownership. They would have the most in the way of events and nightlife, where a PyBer ride may be desired rather than having a designated driver. They would also have the most restrictive and costly parking, so a ride may be preferrable to trying to find parking and paying a high premium. 
3. **Suburban** We would expect suburban cities to fall in between rural & urban in all metrics. Medium population density, medium to high personal vehicle ownership, some amount of events and nightlife, with parking varying by suburb and location within the suburb (for example, a suburb may still have a town center with very limited parking, but ample parking through the rest of the suburb)

### Comparison by city type amongst the 5 key metrics identified
   ![Table Snapshot](https://user-images.githubusercontent.com/85597801/127784829-8e0346f6-cb5c-447a-9b99-6e053beed300.png)


1. **Total Rides** This is highest in urban cities, followed by suburban and rural, in pure volume of rides. This fits with urban cities having more to do, more restricted parking, and a lower percentage of personal vehicle ownership, as well as simply having more people.
2. **Total Drivers** This is highest in urban cities, followed by suburban and rural, again in pure volume. We would expect the total rides & drivers by city type to have a positive correlation- as number of rides go up, number of drivers to provide the rides must also go up. 
3. **Total Fares** This is highest in urban cities, followed by suburban and rural, again in pure volume. We would expect that this also has a positive correlation with total number of rides, as fare is per ride. 
4. **Average Fare per Ride** This is the reverse of the first three metrics- highest among rural, then suburban with urban being the lowest fare. One reason for this may be that the rides tend to be longer in rural areas, as everything is more spread out. Since there are fewer drivers in rural areas, they may also be scarce and able to command a premium on more rides than in urban areas where drivers are plentiful. Urban areas would be the most likely to have short drives, and an abundance of drivers which may be keeping peak pricing low. 
5. **Average Fare per Driver** This matches with average fare per ride, being highest in rural, followed by suburban and with urban being the lowest. If you compare the total ride column and the total driver column, this makes sense. Rural cities saw an average of 1.6 rides per driver, suburban cities 1.28 per driver, and 0.68 rides per driver in urban cities. As urban cities actually have more drivers than rides, it makes sense that they have the lowest per driver, as some at least 780 drivers would have had a fare of $0.00 since they never had a ride. Due to this skew, median may be a better comparison

### Time series data for January through April

![PyBer_fare_summary](https://user-images.githubusercontent.com/85597801/127784857-8d3eca61-650d-4480-afb9-d19d0dc09235.png)


The trend for all three city types is fairly stable, with small variations week to week. The only real correlation between all three types is a slight bump in total fares in the 2nd to the last week in February. One potential cause for this would be falling near Valentine’s Day and couples wanting to go out and not worry about alcohol consumption. 

The suburbs seem to be on an upwards trend towards the end of the period. A potential cause could be spring vacation, very common in the suburbs, and taking a PyBer to the airport rather than deal with long term parking. The rural cities also had a slight peak at the beginning of April, which could be due to a similar phenomenon. 

## Summary

Three recommendations based on the analysis of the data:
1.  There may be a saturation of drivers in the ‘urban’ classified cities, as a number of drivers had zero rides. Consider weeding out those with low review scores or who have not taken any fares to get rid of the excess in drivers. 
2. Perform another data analysis including the population for each city, so we can analyze data on a per capita basis as well as- for example, it’s possible that the total rides & fares are very even between the three types of cities on a per capita basis rather than a raw volume basis. If rural is low on a per capita basis as well, then perhaps we need to encourage more drivers in rural areas to meet needs of customers. 
3. For future data analysis, we should track the distance of the fare as well as the raw value of the fare. In the current data, it is impossible to tell if the fare differences are due to distance differences, or pricing due to driver availability. For example, if the average ride in an urban city is 3 miles, and the average ride in a rural city is 15 miles, the average fare per mile in urban would be $8.17 versus $2.31 per mile for rural, which give us a very different picture of how rates compare. 
