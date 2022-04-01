# Problem Statement:-
Word "HOTEL" as we are familiar with this word and come across with this word very often.What does HOTEL mean? a hotel is a building where travelers can pay for lodging and meals and other service. The hospitality industry is one of the blooming industry all over the world. Hotel operations vary in size, function, complexity, and cost. Most hotels and major hospitality companies have set industry standards to classify hotel types. An upscale full-service hotel facility offers luxury amenities, full-service accommodations, an on-site restaurant, and the highest level of personalized service Small, lower-priced hotels may offer only the most basic guest services and facilities. so in this project we are going to look into the given data and try to analyze it. here we have data for two types of hotels city hotel and resort hotel from the different countries along the guest list and the average daily price.

<img target="_blank" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQvg-N0-ZDG0jMG4Kwif-HV26x1VbAh4ujIug&usqp=CAU.jpg" width=1000; height=300>

# Project Summary
We have been given the data of hotel industry.our first aim to understand the hotel industry "how it
works actually?" and basic terminologies like market segments, distribution channels. In categories, the
term “TA” means “Travel Agents” and “TO” means “Tour Operators” etc.Our second aim is to identify
actionable insights from our data and use basic analysis to give conclusions about key aspect of our data
i.e. cancellation rate, distribution channels, market segment etc.

Our approach towards problem statement was well decided by all three of us. We have been decided
that we will divide the complete project into 10 sub categories that is read data, fill missing values, drop
NA values and duplicates, Identify Continuous and Categorical Variables, detect outlier, replace outlier
with IQR(inter quartile range),univariate analysis, bivariate analysis, correlation of data, hypothesis
questions to get some useful predictions.

We started with importing libraries needed for entire project, after importing we did some basic
analysis like head, tail, describe and info of our data. Doing this we get some knowledge about data. 

Then we focused on our null, missing and duplicate values. We replaced null and missing values with the help of
mean and mode values, for duplicate data we drop all the duplicate data. After doing this we recognized
that in our data there is no use agent and company column. So we dropped those columns. After this there
no more missing, null and duplicates in our data. Then we checked which hotel has more reservation. We
found that city hotel has more reservation than resort hotel. We will try to analysis, why there is huge gap
between these hotels?

We looked into Identifying Continuous and Categorical Variables. It was very helpful, when we
were doing univariate and bivariate analysis. Sometimes identifying categorical and continuous variable
python took object data type also in Continuous variable. While doing this we should have more careful.
As we proceed, we looked into the outlier part for numeric type columns, we Identified the outlier
using boxplot.with the help of IQR we replaced the outlier. Also changed the Continuous Variables which
should be Categorical i.e. PrevBook, PrevCancel.after this we looked outlier for categorical variable using
describe Function and replaced it.

Then we were started with univariate analysis for column canceled, country, meal, segment,
customer data type, year, month and reservation. For this we define function to identify continuous and
categorical variable and for numeric column we use histogram and count plot graph to get some insights.
Then for categorical variable we used pie chart. from this we got some of the following conclusion:-
1) In terms of hotel most number of reservations has city hotel compared to resort hotel.
2) Overall bookings were canceled which is around 27%.
3) Around 31.5% of all bookings were booked from Portugal, Great Britain 12% & France 10%.
4)August is the most occupied or busiest month with 12.9% bookings and January is the most unoccupied
month with 5.36% bookings.
5) Highest number of booking made via online travel agent i.e. 59%, almost 15.8% of bookings are made
via Offline Travel Agents, and less than 15% are Direct bookings without any other agents.
6)48.5% bookings were done in 2016, 36.2% in 2017 and 15% in 2015.
7) BB (Bed & Breakfast) is the most ordered meal which is around 77.7%, followed by SC (no meal
package), HB (Half Board), Undefined and FB (Full Board).
8) Transient (person) type of customers is more around 82%.

Next we did for bivariate analysis. When we talk about bivariate analysis, It means analyzing 2
variables. Since we know there are numerical and categorical variables, there are 3 ways we can analyze
these variable. I) Numerical vs. Numerical II) Categorical vs. Numerical III) Two Categorical Variables. 
In this we used joint plot and bar plot using sea born library.seaborn library has awesome functionality, we
used some of it. From this we got some of the following conclusion:-
1) Maximum number of booking not change by Transient customer and most of Change Booking Done by
Transient-party.
2)Resort Hotel have very less Average Daily Rate(ADR) comparing with City Hotel
3) Both hotels have maximum Previous Booking done by group, followed by transient and transient-party
and very less previous booking had done by contract.
Then we have drawn the correlation heat map to know more about variables. How variable
correlated? Here we see that, the data is highly correlated with PrevBook and Repeat Guest also there is
negative correlation between "Arriving Week" and "Arriving Year".
After this, we have done some hypothesis questions which help us to get more insights and useful
outcome. 
I) Does market segment have any impact on repeated guest?
II) Is effect of customer types and reservation status?

From this we got some of the following conclusion:-
1) While working on first hypothesis question, does market segment have any impact on repeated Guest?
We saw that there are very few people who repeat the same market segment and most of people was not
repeating same market segment.

2) Second hypothesis question, Is effect of customer types and reservation status? The group type check-
out status has more percentage and in cancelled status transient type has more reservation percentage.

Then we started with price analysis part, In that we compared average daily rate on the basis of types
of hotels, types of assigned room and month and years. In hotel vise comparison city hotel has high adr
then that of resort hotel. If we checked on assign room type then H, G and F have high adr also L & P has
negligible adr compared to others. If we check month vise adr then August 2017 has highest adr and the
lowest is November 2015.

## Conclusion: 
Even percentage of total booking more in city hotel as compared to resort hotel but the
number of cancellation in city hotels maximum compared to resort hotel. Overall cancelation rate is 27%.
Approximately 20% of the total booking is getting cancelled in city hotel. Hence the percentage of
confirmed booking is more in resort hotel. The “online TA” is most used market segment and “TA/TO” is
maximum in distribution channel. Transient type of customer is most coming customer compared to other.
