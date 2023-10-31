# Analysis with Pandas on Trending Youtube Video Statistics

> Raahim Khan - Nov 15, 2019

This article is written as a log of our work for our Data Science project. Our project was aimed at analyzing the daily YouTube trending videos data sets that are available here:

[Trending YouTube Video Statistics data set DOWNLOAD](https://www.kaggle.com/datasnaek/youtube-new)

YouTube maintains a list of the top trending videos on the platform. This data set includes several months of data on daily trending YouTube videos. Data is included for the USA, Great Britain, Germany, Canada, France, Russia, Mexico, South Korea, India and Japan. This list is determined by using user interactions such as views, comments and likes to identify which videos are user preferred and displays them on the trending page. Ranking of these videos is done based on a ratio of views, likes, comments and shares, in order to display the best videos at the top of the page. We used the data sets available and began the process of data cleaning followed by Exploratory data analysis (EDA). This article will be divided into two sessions as follows:

- Data Cleaning
- Exploratory Data Analysis
  - Ratio of likes-dislikes in different categories?
  - Users like videos from which category more?
  - Top 5 videos that are on trending in each country?
  - Is the most liked video also the most trending video?
  - Maximum number of days to trending status for a video?
  - Users like videos from which category more?
  - Users comment on which category the most?
  - Frequently occurring words in tags and description
  - and more …

## Data Cleaning