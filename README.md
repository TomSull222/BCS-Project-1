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
