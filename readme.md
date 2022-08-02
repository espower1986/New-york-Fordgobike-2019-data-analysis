## New york Fordgobike 2019 data analysis

### What is bike-sharing ?

>A bicycle-sharing system, is a shared transport service in which bicycles are made available for shared use to individuals on a short term basis. Many bike share systems allow people to borrow a bike from a "dock" and return it at another dock belonging to the same system. [Wikipedia](https://en.wikipedia.org/wiki/Bicycle-sharing_system).


### Dataset

> The dataset analyzed in this report consists of two datasets from two different sources:
>- New York bike share dataset from January  to december 2019, collected from [Bikeshare](https://s3.amazonaws.com/tripdata/index.html), it is a record of various features for every individual bike trips like (date, strat/end trip time, start/end trip station,  user birthyear, gender and type ....) this link provide   
>- New York weather dataset covering the same period, from [(power.larc.nasa.gov)](https://power.larc.nasa.gov/data-access-viewer/) this dataset provide weather informations (temperature, wind speed, humidity, precipitations...)
>- To analyse with total daily rent time we had to generate a new tables using groupby and pivot functions with aggregating numeric features to sum or mean.

### Summary of Findings

In the exploration, I found that most tripe lasts between 2 and 10 minutes, the greatest percentage (about 47.35%) of trips are made by young adult between 17 and 34 years old, with domination of subscribers (89%). I found also that Males are the most frequently observed gender with a percentage of 71%.
Concerning the variation in the number of trips depending on the time period we observe that the greatest number of trips recorded in August and September, on the other hand January, February and December are the months which recorded the lowest number of trips, also  most of the trips are recorded in the morning and evening especially between 07h am and 09h am, and between 16h pm and 20 pm, otherwise less trip count are observed at night.
When I analyzed the trip duration I noticed that the custumers keep the bike for a longer period than the subscribers this may explain a difference use between this two categories. 
Adolescents use bikes for a long time , unlike old ages who shows a shorter duration of use.
The temperature generally varies between 6 ° C and 22 ° C in New York while the humidity generally varies between 71% and 86%.
After analysing the relationship between trip count with differents weather features, we observe that the relationships trip count/Temperature and trip count/humidity is approximately linear but the best feature in predicting the trip count is the temperature.
After analysing the generated tables. I found that the Total daily rent time is strongly and positively related to temperature, not only the daily total rent time but also The ratio of females, the users age averge and custumers ratio are significantly related to temperature.

### Key Insights for Presentation

My priority for the presentation is to visualize the effect of the weather and especially to present the influence of the temperature on the total daily rent time. I started by representing the distribution of the trip duration using histogram, and the different percentages of the user characteristics using pie chart, and to show the relationship between time and the number of trips I used barplot to visualize the peak-to-trough by months, day of week and hours.
the multi scatter-plot allowed to visualize the best weather feature in pridecting the trip daily count which is the temperature. the relationship between temperature and total daily rent time by different user characteristics is visualized by  multiple scatter-plot using color-bars and palettes. To visualize the relation between the temperature and the total daily rent time by type of day I used the scatter-plot by configuring the markers.
