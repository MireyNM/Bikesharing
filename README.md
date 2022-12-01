# Bikesharing
Present a business proposal for a bike-sharing company, using Tableau
## Overview
In this project, we used Pandas and Tableau to analyze data from the Citi Bike program in New York City, for the month of August, in order to create a bike trip analysis. 

### Aim
The aim of this project is create effective visualizations from the Citi Bike data in order to impress potential investors and convince them that a bike-sharing program in Des Moines is a solid business proposal.

## Resources 
- Data Source: 201908-citibike-tripdata.csv.zip from <a href="https://ride.citibikenyc.com/system-data">Citi Bike System Data page</a>
- Software:  Python 3.7.13, Jupyter Notebook, Tableau. 
- Python code: <a href="https://github.com/MireyNM/Bikesharing/blob/main/NYC_Citibike_Challenge.ipynb"> NYC_Citibike_Challenge.ipynb</a>
- Link to Tableau Dashboard: <a href="https://public.tableau.com/app/profile/mireille1519/viz/BikeTripAnalysis_16698722545660/Story1"> Bike Trip Analysis Dashboard </a>

## Results
Using Tableau, we have created the following visualizations:

**1 - NYC Citi Bike General Dashboard**
<p align = "center">
<img width="499" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/109363759/204973649-b40f0d0f-51c5-42cb-b332-bf5088f1263d.png">
</p>
<p align = "center">
Fig.1 - NYC Citi Bike General Dashboard
</p>

Based on Fig.1 we can conclude: 
- Number of trips recorded: 2,344,224 
- Type of users: 1,900,359 trips were checkout by subscribers users and 443,865 by customers.
- Gender of users: 1,530,272 Male - 588,431 Female - 225,521 Unknown. It’s interesting to notice that the number of male users is almost 3 times that of female. 
- We can see that ride duration increases when age decreases. 
- The maps of starting locations and ending locations shows that bike trips are been taking in the whole city which is quite promising.


**2 - How long bikes are checked out for all riders and by gender?**

<p align = "center">
<img width="499" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/109363759/204973703-45756a41-89d8-41d5-87f7-55018206f61d.png">
</p>
<p align = "center">
Fig.2 - Checkout Times for Users 
</p>

- One can notice that the checkout time for all users is mainly under 60min with a peak of 5min use for 146,752 users. 
- As the time increase, the number of users decreases. 
 
<p align = "center">
<img width="499" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/109363759/204973748-86f6663d-88dd-4941-8a66-1870be8d9e5d.png">
</p>
<p align = "center">
Fig.3 - Checkout Times for Users by Gender
</p>

From the above plot, we can conclude: 
- The number of male riders is the highest among all genders. 
- The average of checkout time is approximately the same for both male and female users: male riders have a peak at 5min while female have a peak at 6min. Which indicated that the main reason for using the bikes is short trips. </br>

By unchecking the first Hour Trip Duration and checking larger amount of time, we can notice: 
- The number of riders decreases as the time increases.
- When the amount of time for renting bike increases, the number of rides by male remains higher than that by female. However, the difference in the number of rides between sex becomes relatively smaller.

**3- The number of bike trips by weekday for each hour of the day as a heatmap**

<p align = "center">
<img width="499" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/109363759/204973793-ec4428bb-d34f-4bfb-ae3d-741716748de1.png">
</p>
<p align = "center">
Fig.4 - Trips by Weekday per Hour
</p>

The above heatmap shows:
- The highest number of bike trips is on Thursday.
- The highest number of trips is between 5pm and 7pm of each day of the week. This number decreases as we go after 7pm to reach the the lowest valuesbetween 12am and 4 am.
 
**4- The number of bike trips by gender for each hour of each day of the week as a heatmap**

<p align = "center">
<img width="499" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/109363759/204973843-214faa74-21bf-4157-be46-99ea0057feaf.png">
</p>
<p align = "center">
Fig.5 - Trips by Weekday per Hour for each Gender
</p>

Even though the numbers are higher for male users, the highest number of trips for each gender remains between 5pm and 7pm. 

**5- The number of bike trips broken down by gender for each day of the week by each Usertype**

<p align = "center">
<img width="499" aalt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/109363759/204973912-51060f91-6d2c-4b5c-80bc-6edb5c1117b2.png">
</p>
<p align = "center">
Fig.6 - User Trips by Gender by Weekday
</p>

- In all days of the week, the probability of male checking a bike is higher than that of a female or unknown gender.
- For Subscribers riders, there's no exact trend of which days are busier than others, however we can notice that the biggest number of renting bikes is on Thursday for all the genders.
- While for Customer riders, one can notice that the number of rented bikes is larger during the weekend (Friday to Saturday), for all gender types. Moreover, Saturday is the day with the biggest number of customers' users. Which is logical, considering customer riders must manly be visitors or tourists while subscribers should mainly be local.

**6- The number of bike trips by days of the week** </br>
In order to make sure that Wednesday is the day of the week with the lowest numbers of trips, we have created a heat map to show the number of bike trips in each day of the week. As expected, Thursday is the day with most trips while Wednesday is the day with the lowest number of trips. 

<p align = "center">
<img width="499" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/109363759/204974003-d41e5d46-745e-44aa-8933-503a8509a701.png">
</p>
<p align = "center">
Fig.7 - User Trips by Weekday
</p>

**7- Suggested Days and Times for Repair**

<p align = "center">
<img width="499" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/109363759/204974049-8f2ce65f-d6d8-4b61-b5cb-05a4758e6f76.png">
</p>
<p align = "center">
Fig.8 - User Trips by Weekday
</p>

- Based on Bike Utilization bubble created before, one could check the bikes ID with most utilization time, in order to check them for repairs. 
- By drawing a horizontal bar chart showing the number of bike trips according to each hour of the day and by referring to the heat maps created before we can confirm that the day with the lowest number of rides is Wednesday which could be the best option for bike repairs. While, the hours with the least bike rides are from 9pm to 4am which make these duratin the best one for bike repairs. 

## Conclusion and suggestions

I believe, investing in the bike-sharing program in Des-Moines is a solid business proposal. However, in order to increase the company’s benefits I would suggest: 
- Drawing maps in orders to find any correlation between the number of bike trips and household income. 
- Finding data about bikes types (city bike, mountain bike, kids bike, tandem bikes, tricycle ...) and sizes; In order to answer questions like: Which types and sizes are most rented in general? Which types and sizes are most rented by gender and by weekdays and hours?
- Finding out the reason behind the low number of female renting bikes compared to male, in order to find a solution and increase the number of female users. Maybe, providing child bike trailers will encourage mothers to rent a bike and therefore increase the users number and the company profit.
