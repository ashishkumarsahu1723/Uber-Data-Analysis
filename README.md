# Uber-Data-Analysis
# OBJECTIVE:- To estimate the revenue figure of uber in a year in NY and it's growth and also aimed to expose all the interesting insights that can be derived from a detailed analysis of the dataset.

# What is Data Analysis ?
As MY Project name is Uber Data Analysis so first question comes in our head whats is data analysis like what are the objectives of data analysis so-

Data analysis is defined as a process of cleaning, transforming, and modeling data to discover useful information for business decision-making. The purpose of Data Analysis is to extract useful information from data and taking the decision based upon the data analysis.
A simple example of Data analysis is whenever we take any decision in our day-to-day life is by thinking about what happened last time or what will happen by choosing that particular decision. This is nothing but analyzing our past or future and making decisions based on it. For that, we gather memories of our past or dreams of our future. So that is nothing but data analysis. Now same thing analyst does for business purposes, is called Data Analysis.

# CONTEXT OF ENTIRE PROJECT:-
This uber dataset contains data about Uber’s ridership between September 2014 and August 2015. This dataset contains ~31 million rows and columns of origin, destination, pickup date and time, trip distance, and duration.

The combination of trip distance and duration allows for estimating Uber’s revenue for each trip in NYC. In another hand, the pickup and drop-off locations were anonymized and grouped as taxi zones instead of geographic coordinates. This is a better attempt to preserve data privacy, but it precludes the positioning of such locations on a map.

Before diving into the data, let me clarify what the term “very large” in the title means. The data comprises one complete year of trips, with a total of about 31 million entries. However, some objects will be large enough to require better reasoning about how to efficiently apply transformations to them, from date-time parsing to arithmetic functions.

Here, I did an EDA on the uber dataset, which consisted of data from rides booked in NYC over the course of one year, from September 2014 to August 2015, and eventually computed the income of Uber in one year as well as the revenue trend during the year. This dataset was limited to around 31 million rows and columns of origin, destination, pickup date and time, travel distance and duration.

Used Pandas data frame to check for the presence of null values in the dataset and discovered that the destination column had 1.3 million missing data but that the corresponding data in other columns such as origin, trip duration, trip distance, pickup date and time data were present for these missing data, implying that we cannot remove these missing rows from our dataset because they have a significant impact on Uber's total revenue. Because the destination column was categorical, I utilized the mode imputation approach to address missing values.There were some missing values in the trip length and trip distance columns as well, so I used the mean imputation approach to address these.

Also, feature engineering was used to construct several columns that can help with analysis and expand the area of study. As a result, I made distinct columns for the year, month, and day of the trip. These columns were then utilized to determine the data's monthly trend. Also included a column for trip revenue, which was used to determine total revenue and average revenue. The revenue consisted of various components like:-
. Base fare = 2.55
. per minute = 0.35
. per mile = 1.75
. Minimum fare = 8
# FINDINGS:-
# 1.The effect of time on demand for uber riders: distribution per hour, weekday, and month.
# 2.Estimate monthly base revenue: how much was NYC market worth in the period ?
# 3.Month over month revenue growth: how fast has uber grown in the period ?
# 4.A plot with the total number of trips per day, highlighting some change points assosiated with major holidays and other weather and touristic/cultural events.
# 5.Visualization the most popular pick up and drop off location pairs.
