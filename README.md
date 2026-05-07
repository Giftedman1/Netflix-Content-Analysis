# Netflix-Content-Analysis
A data analysis project exploring Netflix's content library of over 8,800 titles to uncover patterns in content type, genres, countries, ratings, and more.
---
Project Overview
This project analyzes a Netflix dataset sourced from Kaggle to understand how the platform structures its content catalog. The analysis covers everything from content type distribution to the most featured actors across the platform.

---
Objectives

What percentage of Netflix's catalog is Movies and what percentage is TV Shows?
How has the number of titles added to Netflix increased from year to year?
Which countries produce the most content available on Netflix?
What are the most popular content genres on Netflix?
What age ratings are most common across Netflix titles?
How long are most Netflix movies, and what is the typical runtime?
How many seasons do most Netflix TV shows run for?
Which actors appear most frequently across Netflix titles?

---
Dataset
Source: Kaggle — Netflix_Titles
Records: 8,807 titles
Columns: 12
ColumnDescriptionshow_idUnique identifier for each titletypeWhether the title is a Movie or TV ShowtitleName of the contentdirectorDirector of the titlecastActors featured in the titlecountryCountry where the content was produceddate_addedDate the title was added to Netflixrelease_yearYear the content was originally releasedratingAge rating of the contentdurationRuntime in minutes for movies, number of seasons for TV showslisted_inGenre categories the title belongs 
todescriptionBrief summary of the title

---
Tools Used
Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook

---
Data Cleaning Steps
The following issues were identified and fixed before analysis:

Three rows had duration values mistakenly placed in the rating column and were corrected
The date_added column was stored as plain text and converted to datetime format
Trailing whitespace was removed from date_added values
Missing values in rating and country were filled with "Unknown"
Missing values in cast were filled with "Unknown"
The duration column was split into duration_mins for movies and duration_seasons for TV shows
Ten rows with no date_added were excluded only from the library growth visual

---
Key Findings

Movies make up nearly 70% of Netflix's catalog, significantly outnumbering TV Shows
Netflix's library grew rapidly between 2016 and 2019, peaking around 2019 and 2020 before slowing down
The United States leads content production by a wide margin, followed by India
International Movies and Dramas are the most common genres on the platform
TV-MA is the most common age rating, showing Netflix primarily targets adult audiences
Most Netflix movies run between 80 and 120 minutes, with a median of around 99 minutes
The majority of Netflix TV shows run for only one season
Anupam Kher leads all actors with 43 appearances, with the top 10 dominated by Bollywood stars

---
Visualizations

Movies vs TV Shows Distribution
Netflix Library Growth Over Time
Top 10 Countries Producing Netflix Content
Top 10 Most Common Genres
Content Rating Distribution
Movie Runtime Distribution
TV Show Seasons Distribution
Top 10 Most Featured Actors

---
How to Run

Clone this repository
Install the required libraries using pip install pandas matplotlib seaborn
Open Netflix.ipynb in Jupyter Notebook
Run all cells from top to bottom

---
Article
Read the full breakdown of this analysis on Medium: [https://medium.com/@qoozimjamiu21/what-8-800-netflix-titles-tell-us-about-how-the-platform-really-works-a711ba8bd9c1]
