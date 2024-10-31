# Classic Hits Music Dataset Analysis

## Overview

This repository contains an in-depth analysis of a **Classic Hits Music Dataset**, featuring **15,150 tracks** spanning 100 years of music history (1923-2023). It includes files and resources to explore, clean, and analyze data from a wide variety of genres using **Power BI** and **Python**. Each track is enriched with Spotify audio features, enabling insights into musical properties like danceability, energy, tempo, and popularity, all of which help showcase the evolution of popular music across eras.

## Folder Structure

- **Power BI file** (`ClassicHit_Report.pbix`): A report with visualizations and insights on music trends and feature analysis.
- **Excel files**:
  - **Original dataset** (`ClassicHit.csv`): The untouched dataset with raw music data.
  - **Cleaned dataset** (`ClassicHit_Cleaned.csv`): The cleaned and processed dataset, exported from the Python notebook, used in Power BI for analysis.
- **Python notebook** (`data_cleaning_notebook.ipynb`): The Jupyter notebook used to clean and preprocess the original dataset.

## Contents

### 1. Data Preparation (Python Notebook)
In the provided Python notebook, the following data preprocessing steps were conducted:
- **Null and Duplicate Checks**: Identified and removed any rows with null or duplicate values.
- **Genre Refinement**: Simplified genre names for clarity, making analysis more descriptive and consistent.
- **Mode Conversion**: Converted the `Mode` column from numeric values (1 or 0) to descriptive labels ('Major' or 'Minor').
- **Duration Conversion**: Converted the `Duration` column from milliseconds to minutes to improve readability.
- **Exported Cleaned Dataset**: The cleaned data was saved as `ClassicHit_Cleaned.csv` for further analysis in Power BI.

### 2. Data Analysis & Visualization (Power BI)
The **Power BI** report includes several interactive visualizations and insights, providing a detailed look at music characteristics across different time periods and genres. Key analyses include:
- **Yearly Trends of Average Metrics**: Visualizes changes in audio features over time, including popularity, energy, and danceability.
- **Popularity and Duration Analysis**: Examines the relationship between a track’s popularity and its duration.
- **Loudness and Valence**: Explores how loudness correlates with musical positiveness (valence).
- **Energy vs. Danceability**: Analyzes the relationship between energy and danceability, identifying high-energy, danceable tracks ideal for playlists.
- **Total Tracks**: Total track count by genre, year, and artist.
- **Average Energy**: Shows average energy levels by genre or year.
- **Average Danceability**: Displays average danceability levels across time or genres.
- **Average Track Duration**: Provides insights into how track lengths have changed over time.

### 3. Example Insight - HighEnergyDanceable
The **HighEnergyDanceable** metric identifies tracks with both high energy (>0.7) and danceability (>0.7), representing potential "high-energy dance hits." This subset is valuable for understanding trends in party and dance music, helping with playlist creation or trend analysis.

## Usage

1. **Clone the repository** and install necessary dependencies for the Python notebook if applicable.
2. **Run the Python notebook** (data_cleaning_notebook.ipynb) to explore or modify the data cleaning process.
3. **Open the Power BI file** (ClassicHit_Report.pbix) to view, edit, or add visualizations. Make sure the file path to the ClassicHit_Cleaned.csv matches your setup.
