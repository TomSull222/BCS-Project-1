# Exploratory Data Analysis of Films by Year (1980-2017)

## Team Members
- **Dan**
- **Thomas**
- **Prachi**
- **Rashi**

## Project Overview
This project investigates the evolution of filmmaking from the 1980s to the 2010s by analyzing key aspects of films released during this period. The analysis focuses on:

- **Diversity in Filmmaking**: Assessing the representation of women in film production (cast and crew) and exploring its correlation with box office performance.

- **Release Seasonality**: Analyzing the timing of film releases by season and how it correlates with ratings and box office revenue.
  
- **Box Office Performance and Awards**: Evaluating average box office revenues and the number of awards received by films each year.

- **Genre Trends and Film Durations**: Analyzing trends in genre popularity over time and exploring the relationship between film genres and average runtime.


## Research Questions

### Diversity in Filmmaking
- How has female representation in film production (cast and crew) changed from 1980 to 2017?
- What is the correlation between the percentage of women in film production and box office revenue?

### Release Seasonality
- Which seasons tend to yield higher ratings?
- Which seasons show stronger box office performance?

### Box Office Performance and Awards
- What are the yearly averages for box office revenues?
- What are the yearly averages for the number of awards received by films?

### Genre Trends and Film Durations
- What are the most popular genres over the decades?
- How does genre popularity relate to average runtime?

## Data Sources
We will utilize the following datasets:

- **The Movie Dataset** from Kaggle: [The Movie Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset?resource=download)
  - Key files include:
    - `credits.csv`
    - `movies_metadata.csv`

- **OMDb API Dataset**: `omdb_data.csv`
  - Contains additional columns such as Year, Rated, Awards, imdbRating, imdbVotes, etc.

## Team Responsibilities
Each team member will focus on a specific aspect of the analysis:

- **Dan**: Diversity in Filmmaking
- **Thomas**: Release Seasonality
- **Prachi**: Box Office Performance and Awards
- **Rashi**: Genre Trends and Film Duration


## Files and Folder Structure

The project structure includes the following key components:

- **src**: This folder contains the raw data files that supply our datasets for analysis.
  - Files in `src`:
    - `credits_part1.csv`
    - `credits_part2.csv`
    - `movies_metadata.csv`
    - `omdb_data.csv`

- **merged_df.ipynb**: This Jupyter notebook reads the CSV files from the `src` folder, merges them, cleans the data, filters out null values and duplicates, creates new columns calculated from existing data, and converts some columns to the appropriate data types. The output is a file named `merged_df.csv`, which serves as our initial DataFrame for conducting analysis.

- **main.ipynb**: This Jupyter notebook reads in `merged_df.csv` and contains code for calculations and visualizations of our data to address the research questions. The visualizations are saved in the `output` folder.


## Analysis and Conclusion
This exploratory data analysis aimed to uncover trends in the film industry from 1980 to 2017, focusing on diversity in filmmaking, seasonal release patterns, box office performance, awards distribution, and genre patterns.

## Female Representation in Film Production
Our analysis indicates an upward trend in female representation in film production over the decades. The average percentage of female cast members grew from **30.55%** in the 1980s to **36.65%** in the 2010s, marking an increase of approximately 6%. A more dramatic shift occurred among female crew members, whose average representation rose from **11.24%** in the 1980s to **22.97%** in the 2010s, reflecting a pronounced increase of around 11%. This suggests a growing recognition of the need for female voices and perspectives in behind-the-scenes roles. The combined average of female representation (cast and crew) also saw a notable rise from **20.90%** in the 1980s to **29.86%** in the 2010s, indicating an overall improvement in gender diversity across both on-screen and off-screen roles.

We examined the correlation between female representation and box office revenue. Although a scatter plot revealed no significant correlation, our graph, **"Relationship Between Female Representation (Cast + Crew) and Box Office Revenue by Year,"** illustrates that the increase in average combined female representation parallels the growth in box office revenue.

### Key Statistical Analysis
- **Aggregation**: We grouped the data by decade and calculated averages for female representation in cast and crew roles to capture long-term trends.
- **Trend Analysis**: We utilized regression lines to visualize the change in female representation over time, highlighting a positive trajectory for gender diversity.
- **Correlation Analysis**: We computed correlation coefficients to quantify the relationship between female representation and box office revenue. Although the correlation was weak, the visual trend showed a parallel rise in both female representation and revenue.

## Release Seasonality
Our seasonal analysis revealed that **Fall** was the most popular time for film releases, with an average of **1,850 films**, compared to around **1,500** for Spring, Summer, and Winter. However, despite this higher number of releases, Fall had the lowest box office performance, with an average of **$30 million** per film. In contrast, **Summer**, with fewer releases, generated the highest average revenue, nearly **$50 million** per film.

In terms of critical reception, Fall had a slight edge, with an average **IMDb rating of 6.5**, compared to **6.25** for other seasons. However, this difference is minimal, suggesting that higher critical ratings in the Fall do not necessarily translate into box office success.

### Key Statistical Analysis
- **Comparative Analysis**: We compared the number of releases, box office performance, and IMDb ratings across seasons, identifying Fall as the season with the highest number of releases but the weakest box office returns.
- **Averages Calculation**: We summarized data through mean calculations for the number of films, box office revenue, and IMDb ratings per season to provide a clear overview of seasonal performance.
- **Trend Comparison**: By analyzing differences between seasons, we highlighted the disparity between the number of releases and financial success, emphasizing Summer as the most profitable season.

## Box Office Performance and Awards
Examining box office trends, we observed that the **1980s** had stagnant growth, with average annual revenue hovering around **$25 million**. However, in the **1990s**, the film industry gained momentum, with an increase of nearly **$15 million** in average revenue by the end of the decade. This upward trend continued through the **2000s**, with a **$20 million** increase. Although more volatile, the **2010s** still showed an overall growth of around **$10 million** by **2017**.

The trend in award distribution mirrored box office performance, with the **1990s** doubling average awards and steady growth through the **2000s**. Films with IMDb ratings between **7.5 and 9** saw a sharp rise in box office revenue, though some highly rated films earned less, likely due to niche audiences. Awards surged for films rated between **5 and 8**, with more variability beyond that range.


### Key Statistical Analysis
- **Yearly Average Calculation**: We computed yearly averages for both box office revenue and awards, allowing for an examination of trends and fluctuations over time.
- **Comparative Trend Analysis**: By comparing box office performance and awards distribution side by side, we identified that the growth in revenue generally paralleled the increase in awards, showing a broader industry expansion.
- **Growth Rate Assessment**: We quantified the growth rates for both box office revenue and awards by comparing decade-by-decade averages, revealing similarities in their trajectories.

## Genre Trends and Film Durations
An analysis of the total number of films by genre from 1980 to 2017 highlighted **Drama** as the most dominant genre, with over **3,000 films released**. **Comedy** followed with more than **2,500 releases**. While genres like Action and Thriller also had significant representation, Drama and Comedy far outpaced others.

Regarding film durations, genres such as **History, Biography, War, and Western** typically had the longest runtimes, likely due to the complexity of storytelling required. In contrast, **Animation** and **Short films** had the shortest runtimes, fitting their format and target audience.

### Key Statistical Analysis
- **Aggregation by Genre**: We calculated the total number of films released in each genre to identify the most and least prevalent genres from 1980 to 2017, highlighting the dominance of Drama and Comedy.
- **Runtime Analysis**: We calculated average runtimes for each genre, using mean values to illustrate the disparity between long-format genres (History, Biography, etc.) and shorter formats (Animation, Shorts).
- **Comparative Analysis**: By comparing genres based on the total number of films and their average runtime, we emphasized the contrasting nature of these categories in terms of both volume and storytelling depth.

