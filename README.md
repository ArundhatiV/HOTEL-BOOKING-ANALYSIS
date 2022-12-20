# HOTEL-BOOKING-ANALYSIS

# Hotel Bookings Exploratory Data Analysis

## Objective
We are provided with a hotel bookings dataset. 

Out main objective is perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.

## Dataset
We are given a hotel bookings dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.

```
- 




- Total number of rows in data: 119390
- Total number of columns: 32
## Data Cleaning and Feature Engineering

### (1) Removing Duplicate rows
All duplicate rows were dropped.

### (2) Handling null values
- Null values in columns `company` and `agent` were replaced by 0.
- Null values in column `country` were replaced by 'others'.
- Null values in column `children` were replaced by the mean of the column.
  

### (3) Converting columns to appropriate data types

- Changed data type of `children`, `company`, `agent` to int type.
- Changed data type of `reservation_status_date` to date type.

### (4) Removing outliers

- One outlier was found in the `adr` column. Simply dropped it.

### (5) Creating new columns
- Created new column `total_stay` by adding `stays_in_weekend_nights`+`stays_in_week_nights`.
- Created new column `total_people` by adding `adults`+`children`+`babies`.

## Exploratory Data Analysis

Performed EDA and tried answering the following questions:

```
 Q1) Which agent makes the most no. of bookings?
 Q2) Which room type is in most demand and which room type generatesthe  highest adr?
 Q3) Which meal type isthe  most preffered meal of customers?
 Q4) What isthe  percentage of bookings in each hotel?
 Q5) Which is the most common channel for booking hotels?
 Q6) Which are the most busy months?
 Q7) From which country most of the guests are comin ?
 Q8) How long do people stay at the hotels?
 Q9)  Which hotel seems to make more revenue?
 Q10)  Which hotel hasa  higher lead time?
 Q11)  What is preferred stay length in each hotel?
 Q12)  Which hotel has higher bookings cancellation rate.
 Q13)  Which hotel hasa  high chance that its customer will return for another stay?
 Q14)  Which channel is mostly used forthe  early booking of hotels?
 Q15)  Which channel hasa  longer average waiting time?
 Q16)  Which distribution channel brings betterrevenue-generatingg deals for hotels?
 Q17)  Which significant distribution channel has the highest cancellation percentage?
 Q18) Doesa  longer waiting period or longer lead time causes the cancellation of bookings?
 Q19) Whether not getting allotted the same room type as demand is the main cause of cancellation for bookings?
 Q20) Does not alloting the  same room as demanded affect adr? 
 Q21) What is the trend of bookings within a month?
 Q22) Which types of customers mostly make bookings?

```

Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:
  -  Bar Plot.
  -  Histogram.
   - Scatter Plot.
   - Pie Chart.
   - Line Plot.
   - Heatmap.

             
###  Univariate Analysis:

Performed univariate analysis and made following conclusions:
```
 1.) Agent no. 9 has made most no. of bookings.
 2.) Most demanded room type is A, but better adr generating rooms H, G and C. Hotels should increase the no. of room types A and H to maximise revenue.
 3.) Most popular meal type is BB(Bed and Breakfast).
 4.) Around 60% bookings are for City hotel and 40% bookings are for Resort hotel, therefore City Hotel is busier than Resort hotel.
 5.) Guests use different channels for making bookings out of which most preferred way is TA/TO.
 6.) July- August are the most busier and profitable months for both of hotels. 
 7.) Most of the guests came from european countries, with highest number of guests from Portugal.
 8.) Most common stay length is less than 4 days and generally people prefer City hotel for short stay, but for long stays, Resort Hotel is preferred.
 
```




### Bivariate Analysis :

We tried to answer following questions
```
 1.) Overall adr of City hotel is slightly higher than Resort hotel and no. of bookings of City hotel is also higher than Resort hotel. Hence, City hotel is makes more revenue.
 2.) City hotel has slightly higher median lead time. Also median lead time is significantly higher for both hotels, this means customers generally plan their hotel   visits way early.
 3.) Almost 30 % of City Hotel bookings got canceled.
 4.) Both hotels have very small percentage that customer will repeat, but Resort hotel has slightly higher repeat % than City Hotel.
 5.) TA/TO is mostly used for planning Hotel visits well ahead of time. 
 6.) While booking via TA/TO one may have to wait a little longer to confirm booking of rooms.
 7.) GDS channel brings higher revenue generating deals for City hotel, in contrast to that most bookings come via TA/TO. City Hotel can work to increase outreach on GDS channels to get more higher revenue generating deals.
 8.) TA/TO has highest booking cancellation %. Therefore, a booking via TA/TO is 30% likely to get cancelled.
 9.) Longer lead time has no affect on cancellation of bookings.
 10.) Not getting same room as demanded is not the case of cancellation of rooms. A significant percentage of bookings are not cancelled even after getting different room as demanded.
 11.) Not getting same room do affects the adr, people who didn't got same room have paid a little lower adr. 
 12.) Arrivals in hotels increases at weekends and also the avg adr tends to go up as month ends. 
 13.)Moslty bookings are done by couples(bookings have two adults.)
```

## Conclusion
```
 1.)City hotels are the most preferred hotel type by the guests. We can say City hotel is the busiest hotel.
 2.)27.5 % bookings were got cancelled out of all the bookings.
 3.)Only 3.9 % people were revisited the hotels. Rest 96.1 % were new guests. Thus retention rate is low.
 4.)The percentage of 0 changes made in the booking was more than 82 %. Percentage of Single changes made was about 10%.
 5.)Most of the customers (91.6%) do not require car parking spaces.
 6.)79.1 % bookings were made through TA/TO (travel agents/Tour operators).
 7.)BB( Bed & Breakfast) is the most preferred type of meal by the guests.
 8.)Maximum number of guests were from Portugal, i.e. more than 25000 guests.
 9.)Most of the bookings for City hotels and Resort hotel were happened in 2016.
 10.)Average ADR for city hotel is high as compared to resort hotels. These City hotels are generating more revenue than the resort hotels.
 11.)Booking cancellation rate is high for City hotels which almost 30 %.
 12.)Average lead time for resort hotel is high.
 13.)Waiting time period for City hotel is high as compared to resort hotels. That means city hotels are much busier than Resort hotels.
 14.)Resort hotels have the most repeated guests.
 15.)Optimal stay in both the type hotel is less than 7 days. Usually people stay for a week.
 16.)Almost 19 % people did not cancel their bookings even after not getting the same room which they reserved while booking hotel. Only 2.5 % people cancelled the booking.
```

## Summary
```
1)Majority of the hotels booked are city hotel. Definitely need to spend the most targeting fund on those hotel.
2)We also realise that the high rate of cancellations can be due high no deposit policies.
3)We should also target months between May to Aug. Those are peak months due to the summer period.
4)Majority of the guests are from Western Europe. We should spend a significant amount of our budget on those area.
5)Given that we do not have repeated guests, we should target our advertisement on guests to increase returning guests.


```
## Suggestions:
```
Inferences and Conclusion
1)Firstly, higher lead time has higher chance of cancellation. Also, history of previous cancellations increases chances of cancellation.
2)Secondly, The City hotel has more guests during spring and autumn, when the prices are also highest, In July and August there are less visitors, although prices are lower. Thus, customers can get good deal on bookings in July and August in city hotel.
3)Guest numbers for the Resort hotel go down slighty from June to September, which is also when the prices are highest. Thus, these months should be avoided for bookings.
4)Thirdly, Broadly, Arpil to August is the peak season of bookings. Both hotels have the fewest guests during the winter.
5)Fourthly, No deposit cancellations are high compared to other categories but these should not be discouraged per se as bookings in this category are also very high compared to non refundable type bookings.
6)Fifthly, cancellations are high when done through agents compared to direct bookings. Hotels need to do marketing and give special incentives for direct bookings as these may establish personal one to one relationships promoting customer loyalty.
7)The cancelled vs. non-cancelled bookings ratio for City Hotel was different than Resort Hotel. It can be established that the type of hotel can play a factor while determining reasons for cancellations.
8)The majority of bookings for both hotels had no deposit collected (rather than partial or full). The same majority is demonstrated in cancelled bookings for both hotels as well.
9)If we just look at non-cancelled bookings data, we can conclude that if people were to cancel more, the majority of the cancellations would be the ones with no deposit collected.
10)It is possible that guests tend to cancel less after paying some deposit. Some sort of deposit collection (partial or full or credit card detail requirement) at booking may reduce overall cancellations.
11)Third-party cancellations are higher than direct hotel bookings, although there is no significant difference in average daily rates.
12)More direct hotel bookings (with offers/discounts) could lead to lower cancellations. The data does not point to an ideal daily rate to use.
13)Non-repeat guests make most of the cancelled and non-cancelled bookings (especially weekday bookings).
14)Conversion of non-repeat to repeat loyal customer base (staying during the week) could lead to lower cancellations.
15)For non-direct bookings (majority of cancellations - City Hotel), months with higher cancellations generally had a higher average daily rate. The same cannot be proved conclusively for direct bookings.

```
## Challenges
```

(1) There was a lot of duplicate data.
(2) Data was present in wrong datatype format.
(3) Choosing appropriate visualization techniques to use was difficult.
(4) A lot of null values were there in the dataset.


