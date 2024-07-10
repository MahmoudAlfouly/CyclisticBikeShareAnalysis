# CyclisticBikeShareAnalysis

## Objective
This project aims to analyze the Cyclistic bike share data to understand usage patterns and provide insights to increase the conversion of casual riders into subscribers.

## Dataset Description
The dataset used for this analysis includes information about bike bike rides taken by Cyclistic customers and subscribers. Some columns are:
1. 'trip_id': identifier for each single trip.
2. 'bike_id': identifier for the bike used in the trip.
3. 'from_station_name', 'to_station_name': start and end stations.
4. 'usertype': Customer (casual rider) or Subscriber (annual member).
5. 'gender', 'birthyear': demographic information about the rider.

## Importance of the Analysis:
Converting casual riders to subscribers is crucial for Cyclistic as it provides a steady stream of revenue and enhances customer loyalty. By understanding the factors that influence casual riders' decisions, we can devise targeted marketing strategies to increase subscriptions.


## Project Steps

1. **Data Loading and Cleaning**
   - Loading the dataset.
   - Handling missing values.
   - Checking for duplicates.
   - Converting data types to the appropriate ones, like converting 'tripduration' and 'birthyear'to numeric.

2. **Exploratory Data Analysis**
   - Summary statistics.
   - Visualization of trip duration.
   - Analysis of trips by time of day, user type, gender, and start/end stations.
   - Getting insights from each analysis.

3. **The More Specific Analysis**
   - Proportion of trips by each uesr type in each day of the week and then the absolute number of trips by each user type in each day of the week.
   - Distribution of trip duration by user type and the distribution of trip duration by user type in each day of the week.
   - The number of trips by each user type.
   - The top start and end stations for each user type.
   - Age distribution by user type.
   - Peak hours for trips by user type.
   - Gender distribution by user type.

## Key Insights

1. **Trip Duration**: Most trips are relatively short, with a significant peak around a few hundred seconds. This suggests that the majority of users are using the bikes for short commutes or quick trips.
2. **Trips Peak Times**: Most trips peak times are in accordance with commuting times (around nine a.m and five p.m).
3. **User Types**: Most users are subscribers with over 300,000 subscribers. Customers are a minority.
4. **Gender**: Most users are male, with more than 250,000 users. Females are a lot less than males, with just over 50,000 users. A proportion of the users have don't have data for 'gender' (missing values) as already calculated in the data cleaning segment.
5. **Trips Weekly Distribution**: The number of trips taken by subscribers is almost stable throught week days (Monday to Friday) and then decreases in weekends (Saturday and Sunday), which would suggest commuting. On the other hand, customers trips were at their highest on weekends and less so on weekdays.
6. **Trip Duration by User Type**: Customers (casual riders) trips take longer durations than members.
7. **Weekly Trip Duration**: For subscribers, the average trip duration is almost stable in each day of the week. For customers, the day with the lenghtheist trips is Thursday.
8. **Trip Count**: The majority of trips are from subscribers with 341906 trips. Customers took 23163 trips.
9. **Top Stations**: For subscribers, the top stations (start and end) are: 'Clinton St & Washington Blvd', 'Clinton St & Madison St' and 'Canal St & Adams St'. While for customers, the top stations (start and end) are: 'Streeter Dr & Grand Ave', 'Lake Shore Dr & Monroe St', 'Millennium Park' & 'Shedd Aquarium'. These stations should be targeted with ads for customers to be converted to subscribers.
10. **Trip Duration Distribution**: Customers take longer duration trips than Subscribers as most trips that are longer than 1500 seconds are taken by customers. On the other hand, most subscribers trips are less than 1000 seconds.
11. **Missing Birthyear Data**: The 'Customer' data is missing a lot (about three quarters) of 'birthyear' data. The company should try to gather more birthyear data from customers.
12. **Age Distribution**:Younger people are more likely to be 'Customer' while older people are more likely to be 'Subsciber'. Most people below thirty years are Customers. Most people older than sixty years are Subscibers.
13. **Peak Trip Times by User Type**: Subscribers are most likely to take trips at the times of going to and leaving work (nine and five). Customers trips are usually between 10 am and 7 pm. They peak at around 3 pm.
14. **Gender Participation**: Predominantly Male Subscribers. Low Female Participation in both usertypes. High Percentage of unknown gender among customers.

## Recommendations:

1. Weekend Advertising: Focus advertising efforts on weekends (Saturdays and Sundays), as these are the peak days for customer trips.
2. Target Key Stations: Place ads at top customer start and end stations such as 'Streeter Dr & Grand Ave', 'Lake Shore Dr & Monroe St', and 'Shedd Aquarium'.
3. Highlight Subscription Benefits: Emphasize the financial advantages of subscribing, particularly for users who take longer trips.
4. Youth-Centric Campaigns: Target younger audiences, especially those under thirty, as they form the majority of the customer base.
5. Peak Hour Advertising: Schedule ads around 3 p.m., which is the peak time for customer trips.
6. Data Collection Improvement: Implement strategies to collect comprehensive gender and birthyear data from customers to enhance future analyses.

## How to Run the Code

1. Ensure you have Python and the necessary libraries installed (`pandas`, `numpy`, `matplotlib`, `seaborn`).
2. Download the dataset and place it in the appropriate directory.
3. Run the Jupyter Notebook or Python script containing the analysis code.

```python
# Example to run the code
import pandas as pd

# Load the dataset
df = pd.read_csv('Divvy_Trips_2019_Q1.csv')

# Proceed with data cleaning and analysis as shown in the provided script
