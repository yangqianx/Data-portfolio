# Netflix Series Dashboard

## 1. Project Overview
This project scrapes data from Rotten Tomatoes to analyze the top 100 Netflix series according to their rankings, genres, actors, and other relevant attributes. The goal is to visualize and analyze trends in Netflix content, providing insights into audience preferences, genre popularity, and the relationship between ratings and rankings.

## 2. Data Sources
The data for this project is scraped from the "100 Best Netflix Series to Watch Right Now" webpage on Rotten Tomatoes (URL: https://editorial.rottentomatoes.com/guide/best-netflix-shows-and-movies-to-binge-watch-now/). This page contains information about the top 100 Netflix series, including:
- Title
- Year of release
- Genre
- Ranking
- Tomatometer score
- Actors
- Links to individual movie pages

## 3. Technologies Used
- **R** for data scraping and data manipulation
  - Packages: `httr`, `xml2`, `rvest`, `dplyr`, `ggplot2`
- **Power BI** for data visualization

## 4. Project Implementation

### Data Scraping
The project starts by scraping the top 100 Netflix series data from the Rotten Tomatoes webpage. The scraper extracts the following information for each series:
- **Title**: Name of the Netflix series
- **Year**: Year of release
- **Genre**: Genre(s) of the series
- **Ranking**: Position in the "Top 100" list
- **Tomatometer Score**: Rotten Tomatoes critic score
- **Actors**: Main actors of the series
- **Links**: Link to the individual Rotten Tomatoes page

### Data Cleaning and Manipulation
Once the data is extracted, it's cleaned to remove unwanted characters, handle missing values, and format the data for further analysis. This includes:
- Cleaning the year and actor data
- Removing unnecessary characters from text fields
- Structuring the genre data for easier analysis

### Data Visualization
The final dataset is imported into Power BI for visualization. Key visualizations include:
- **Genre distribution**: A bar chart showing the frequency of each genre in the top 100 series.
- **Top Netflix series**: A ranking visualization showcasing the highest-ranked series based on Tomatometer scores.
- **Year vs Rating**: A scatter plot showing the relationship between the release year and Tomatometer score.
