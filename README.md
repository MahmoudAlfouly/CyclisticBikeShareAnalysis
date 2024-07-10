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

1. **Trip Duration**: Most trips are short, with a peak around a few hundred seconds, suggesting usage for short commutes or quick trips.
2. **Trips Peak Times**: Trips peak around commuting times (9 AM and 5 PM).
3. **User Types**: Most users are subscribers (over 300,000), while customers are a minority.
4. **Gender**: Most users are male (over 250,000), with a significant number of unknown gender entries.
5. **Trips Weekly Distribution**: Subscriber trips are stable on weekdays and drop on weekends, indicating commuting patterns. Customer trips peak on weekends.
6. **Trip Duration by User Type**: Casual riders take longer trips than subscribers.
7. **Weekly Trip Duration**: Subscribers' average trip duration is stable, while customers' longest trips occur on Thursdays.
8. **Trip Count**: Subscribers dominate with 341,906 trips compared to customers' 23,163 trips.
9. **Top Stations**: Key stations for subscribers and customers differ, suggesting targeted advertising opportunities.
10. **Trip Duration Distribution**: Longer trips are primarily by customers; subscribers' trips are generally shorter.
11. **Missing Birthyear Data**: A significant portion of customer data lacks birthyear information.
12. **Age Distribution**: Younger people are more likely to be customers, while older people are more likely to be subscribers.
13. **Peak Trip Times by User Type**: Subscribers peak during commuting hours; customers peak at around 3 PM.
14. **Gender Participation**: High male participation among subscribers; low female participation in both user types.

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
