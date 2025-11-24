# Riding-Towards-Success-Bikeshare-Analysis
## Analyzing 12 months of Cyclistic bike-share data to identify patterns between casual riders and annual members

## Project Goal:

### The primary objective is to understand how casual riders and annual members use Cyclistic bike-share services differently. This analysis aims to recommend strategies to convert casual riders into annual members.

## Data Source and Tools:

### Data Source: 12 months (April 2020 – March 2021) of public trip data provided by Motivate International Inc. (Divvy/Cyclistic).

## Tools:

### Python: Data cleaning, transformation, and manipulation.
#### Pandas: Data structuring and aggregation
#### Matplotlib & Seaborn: Data Visualization 

## Data Cleaning and Preparation:

### The raw dataset contained over 3.4 million rows across 12 monthly CSV files. Key cleaning steps included:

Merging: Combined all 12 monthly files into one master DataFrame.

Data Type Conversion: Converted started_at and ended_at to datetime objects.

Feature Engineering: Created new columns for:

ride_length_seconds (Calculated duration).

day_of_week, month, and pick_hour.

Anomaly Removal: Filtered out rides with a duration less than 1 second (negative or zero time), which accounted for approximately 10,938 erroneous rows.

Simplification: Removed sensitive geospatial columns (lat, lng) after calculating ride length.

## Key Analytical Insights

The analysis highlights four distinct areas where casual riders behave differently than members:

1. Ride Duration (The Long-Haul Rider)

Insight:

Casual riders use the service for longer, likely leisure trips (tourism, sightseeing) rather than practical commuting.

Median Ride Length

Consistently higher

Low and steady

The average ride length is not skewed by outliers; casual trips are fundamentally longer.

2. Weekly and Hourly Trends (The Weekend Traveler)

Weekly Usage: Member usage remains high and consistent throughout the week, suggesting habitual commuting. Casual usage peaks dramatically on Saturdays and Sundays, indicating leisure, fitness, or social use.

Hourly Usage: Both groups peak during the afternoon (14:00 - 18:00), but the casual peak on weekends is significantly higher in volume.

3. Seasonal Patterns (The Fair-Weather Rider)

Engagement: Total ridership for both groups peaks in the summer months (June-September).

Winter Drop-off: Casual rider engagement drops drastically in the winter (December-February) compared to members, who maintain a higher baseline ridership for essential travel.

4. Station and Bike Preferences (The Docked Bike Preference)

Bike Type: Casual riders demonstrate a strong preference for "Docked Bikes" and use them for the longest durations. This suggests they rely on established, major stations and prefer traditional equipment.

Top Stations: The top 10 starting stations for casual riders are typically located near high-traffic tourist attractions (e.g., parks, museums, lakefront).

🚀 Recommendations for Conversion

Based on these distinct behavioral patterns, Cyclistic should target casual riders with marketing strategies that leverage their weekend, leisure, and seasonal habits:

Flexible Membership Tiers: Introduce a "Weekend Warrior Pass" or a "Seasonal Pass" (e.g., 6-month summer pass) that is more cost-effective than a single ride but cheaper than a full annual membership.

Location-Based Promotions: Place prominent signage and staff at the top 10 casual starting stations (identified in the analysis) offering immediate, time-sensitive membership discounts.

Leisure-Focused Value Proposition: Shift marketing language away from "commuting convenience" to "Leisure Freedom" and "Exploration"—highlighting the cost savings over multiple long rides during a weekend trip.

E-Bike Promotion: Since casual riders prefer long trips, promoting the value of the E-Bike (where available) as part of a membership could entice them to subscribe for comfort on long-distance leisure rides.

Code implemented by J.Favreau, Data Analyst.
