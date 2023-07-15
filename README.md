# Investigate Hotel Business using Data Visualization
- Consists of 119,390 rows and 29 columns
- There is a target column
- Make the results of hotel business performance investigations.
- The dataset contains travel and lodging information, cancellation information, types of deposits that are often used, and types of customers who often stay.
## Data Processing
- Handle missing data.
- Delete unused columns
- Checking the suitability of data types in the dataset.
- Change column values ​​that do not match.
- Perform visualization of data that has been cleaned.
### Here are some visualizations and insights from the data.
1. Data imbalance<br>
![Feature Dependent](https://github.com/NurulIlahiHusnah/Investigate-Hotel-Business-using-Data-Visualization/assets/125198828/d9d6f31d-b6f8-420e-8ce9-f9a8bfd6f095)
2. Chart Hotel<br>
![Distribution Hotel](https://github.com/NurulIlahiHusnah/Investigate-Hotel-Business-using-Data-Visualization/assets/125198828/bc9f80e8-c15c-4bdd-ad3e-6f7763147945)
3. Chart Deposit Type<br>
![Deposit Type](https://github.com/NurulIlahiHusnah/Investigate-Hotel-Business-using-Data-Visualization/assets/125198828/764decce-1452-41fa-bf56-fe17c011423d)
4. Chart Meal<br>
![Distribution Meal](https://github.com/NurulIlahiHusnah/Investigate-Hotel-Business-using-Data-Visualization/assets/125198828/b982bbe9-959e-4968-bbe5-3ff6381323e1)
5. Chart Market Segment<br>
![Distribution Market Segment](https://github.com/NurulIlahiHusnah/Investigate-Hotel-Business-using-Data-Visualization/assets/125198828/ea2f0734-2868-44a2-a112-96b8f8ea3350)
6. Customer Type<br>
![Distribution Customer Type](https://github.com/NurulIlahiHusnah/Investigate-Hotel-Business-using-Data-Visualization/assets/125198828/6a1caf34-f383-4a6c-95b8-0d2d7528c922)
### Result Investigation and Recommedation
1. Impact Analysis of Stay Duration on Hotel Bookings Cancellation Rates<br>

Hotel | Duration Status | is canceled | Duration Rasio 
--- | --- | --- | ---
City Hotel | A day | 31618 | 71.495116   
City Hotel  |     A month     |     179     |    0.404758    
City Hotel  |      A week     |     1295    |    2.928274    
City Hotel  |  Several month  |      10     |    0.022612    
Resort Hotel |      A day      |     7758    |    17.542511   
Resort Hotel |     A month     |     305     |    0.689671    
Resort Hotel |      A week     |     3053    |    6.903491    
Resort Hotel |  Several month  |      6      |    0.013567 

<br>

![Analisa Stay Duration](https://github.com/NurulIlahiHusnah/Investigate-Hotel-Business-using-Data-Visualization/assets/125198828/add3dfad-7985-49a7-be22-a73d107c9d91)


==For Stay duration analysis of canceled hotel bookings, for visitors who stay in the A day category or less than one week, they cancel more hotel orders, this requires further analysis of the causes. Possible temporarily there is a lack of hotel service levels, high prices, flexibility of reservations or indeed because of the destination.

2. Monthly Hotel Booking Analysis Based on Hotel Type <br>


| hotel | arrival_date_month | Total_customer | Duration Rasio |
|------:|-------------------:|---------------:|:--------------:|
|     4 |         City Hotel |        January |    2178.500000 |
|    16 |       Resort Hotel |        January |    1218.500000 |
|     3 |         City Hotel |       February |    2066.000000 |
|    15 |       Resort Hotel |       February |    1324.000000 |
|     7 |         City Hotel |          March |    1868.000000 |
|    19 |       Resort Hotel |          March |    1096.500000 |
|     0 |         City Hotel |          April |    2482.500000 |
|    12 |       Resort Hotel |          April |    1551.500000 |
|    20 |       Resort Hotel |            May |    1668.000000 |
|     8 |         City Hotel |            May |    3229.000000 |
|     6 |         City Hotel |           June |    3740.000000 |
|    18 |       Resort Hotel |           June |    1804.500000 |
|     5 |         City Hotel |           July |    4116.000000 |
|    17 |       Resort Hotel |           July |    1779.500000 |
|     1 |         City Hotel |         August |    3947.000000 |
|    13 |       Resort Hotel |         August |    1522.500000 |
|    11 |         City Hotel |      September |    2696.000000 |
|    23 |       Resort Hotel |      September |    1524.333333 |
|    22 |       Resort Hotel |        October |    1631.333333 |
|    10 |         City Hotel |        October |    2994.333333 |
|     9 |         City Hotel |       November |    3700.000000 |
|    21 |       Resort Hotel |       November |    1554.000000 |
|     2 |         City Hotel |       December |    3802.500000 |
|    14 |       Resort Hotel |       December |    1777.500000 |

<br>

![total customer](https://github.com/NurulIlahiHusnah/Investigate-Hotel-Business-using-Data-Visualization/assets/125198828/2d71af1a-3d5b-4b44-a684-d1e538f1b91f)


== From the visualization above, it is illustrated that the average visitor prefers to use a City hotel compared to a Resort Hotel. Then, judging from the holiday distribution, there are 3 phases where there are Low Season, High Season, and lastly Peak Season. This is reflected in the higher level of visitors in High Season where in Indonesia that month is the period of school holidays, religious holidays such as going home and many other types of holidays that month. At the beginning of August there was a decrease where the holiday period was starting to end, but it would be followed by an increase in November and Dec where in those months there were Christmas and New Year Holidays.

3. Impact Analysis of Lead Time on Hotel Bookings Cancellation Rate<br>
   

<br>

![Analisi stay lead](https://github.com/NurulIlahiHusnah/Investigate-Hotel-Business-using-Data-Visualization/assets/125198828/c20283d4-36cf-4c59-843a-9e6c27ffc2c2)

== For the analysis of the order-to-check-out period (lead_time) for cancellations, it shows a high increase in bookings with durations of 1 hour and above for the whole. There needs to be a new policy to determine the right decision for lead_time duration. To avoid canceling hotel bookings. For temporary assumptions the causes of cancellations with lead_time above 1 hour are:
- Marketing strategy
- Room Availability Planning
