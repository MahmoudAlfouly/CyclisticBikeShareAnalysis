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


## Project Steps

1. **Data Loading and Cleaning**
   - Loading the dataset.
   - Handling missing values.
   - Converting date columns to datetime.
   - Creating additional columns (e.g., age & trip duration).

2. **Exploratory Data Analysis**
   - Summary statistics.
   - Visualization of trip duration.
   - Analysis of trips by time of day, user type, gender, and start/end stations.

3. **Advanced Analysis**
   - Distribution of trip duration by user type.
   - Age distribution by user type.
   - Peak hours for trips by user type.
   - Gender distribution by user type.

## Key Insights

  - **Trip Duration**: Casual riders tend to take longer trips compared to subscribers.
  - **User Type Distribution**: The majority of rides are taken by subscribers.
  - **Age Distribution**: Older individuals are more likely to be subscribers.
  - **Peak Hours**: Subscribers peak during commuting hours (9 AM and 5 PM), while casual riders peak in the afternoon.
  - **Gender Distribution**: There is a high percentage of male subscribers, with low female participation in both user types.

## Recommendations:

  - n

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
