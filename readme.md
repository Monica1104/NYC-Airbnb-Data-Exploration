# New York City Airbnb Data Exploration
## by Jingwen Yi


## Dataset

This dataset is downloaded from Kaggle. It's from the website [New York City Airbnb Open Data](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data). This dataset includes around 50,000 listings in NYC area with 16 columns.

In the data wrangling process, I identified a few items to be cleaned. I dropped all unnecessary columns (`name`,`host_name`, `last_review`). Then I Changed data types for `neighbourhood_group`,`neighbourhood`,`room_type` from object(string) to categorical data. Third step is Filling all NA values in `reviews_per_month` as 0. Lastly, I dropped all listings with price as 0.

## Summary of Findings

In the exploration, I have a few findings.
- Manhattan takes on the highest total listings, followed by Brooklyn. The total listing is more than 20,000 for Manhattan, and is around 20,000 for Brooklyn. Queens' listings number ranks third, but it's significantly much lower than the previous 2.
- Looking at total listings by room type, Entire home/apt is the most common one.
- Price is always the one metric that probably requires 'log' treatment since it always show a long tail on the right. After the logarithmic scale transformation, I found that the most common price is around 100 dollars/night.
- Entire home/apt takes the highest price compared to the other two categories.
- Manhattan's median price is the highest which is in line with the level of prosperity.




## Key Insights for Presentation

For the presentation, I focus on the relationship between price and other numeric metrics, like number of reviews and minimum nights. I started by introducing the distribution of price, then plot the scatterplot.

Afterwards, I introduce key categorical variables like room type and neighbourhood group by plotting boxplots between them and prices. In light of longtitude and latitude info we have, I plot a map with price distribution.

## Licenses
These project does not require any licenses. 
