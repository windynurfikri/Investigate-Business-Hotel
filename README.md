# Investigate-Business-Hotel
Investigate Business Hotel using Data Visualization
<br>
<br>“It is very important for a company to always analyze its business performance. On this occasion, we will explore the business in the hospitality sector. Our focus is to find out how we behave in making hotel reservations, and its effect to the hotel bookings rate. The results of the insights we find will be presented in data visualizations to make it easier to understand and more persuasive. ”
<br>
## Overview
The dataset has 119,390 rows and 29 columns with 9 categorical variable and 20 numerical variable.
Here's whats were found after basic checking, and the steps will be performed to handle it:
- 33,621 duplicated rows, will be dropped
- `company` has so many (>90%) missing/null values.
- Impute missing value in `children` with 0 and change its data type into 'int64', because it must be integer and its mean/median is around 0.
- Impute missing value in `agent` with 0.
- `city` has many categorical value, will be dropped.
- Replace 'Undefined' in `meal` with 'No Meal'.
## Investigation
![image](https://user-images.githubusercontent.com/108982784/184543178-8a9d98e3-bbeb-4f60-833b-3427fc44a05a.png)
- More people choose City Hotel than Resort Hotel. This could be caused by Resort Hotel’s location. Mostly Resort Hotels is located near tourist attractions, which is far from the downtown. So, it is only reserved by people who are on vacation.
- Even City Hotel and Resort Hotel have significant fluctuation differences, but overall, booking’s trend starts growth in April, and July is the month with the highest bookings, this is also related to Mid-year holidays.
- The Cancellation rate can be impacted by Stay Duration and Lean Time.
- In City Hotel, the longer stay duration, the higher cancellation rate can be. Meanwhile, in Resort Hotel the cancellation growth only happens until the week 4 of stay duration.
- Probability of booking cancellation caused by Lead Time usually occurs if more than 270 days (entering the 4th quarter).
