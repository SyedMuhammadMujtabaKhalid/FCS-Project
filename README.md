# Trending YouTube Dataset Analysis - FCS 2025-26 Project 1

## Overview
This repository contains a Jupyter Notebook project for analyzing the "Trending YouTube Dataset". The project downloads and decompresses YouTube trending data across multiple countries, concatenates it into a single Pandas DataFrame, and performs various data manipulations, aggregations, and analyses.

## Features
- **Data Collection & Decompression**: Automatically downloads `.csv.zst` files for 10 different countries from a GitHub repository, decompresses them in memory using `zstandard`, and loads them into Pandas.
- **Data Cleaning**: Formats dates, handles missing values, and excludes videos with disabled comments or ratings.
- **Data Analysis**: 
  - Extracts and filters tags to identify top trending keywords.
  - Groups data by `channel_title` to find the most viewed channels.
  - Computes `like_ratio` (likes/dislikes) for videos and specific tags.
  - Aggregates videos by publish time intervals.
  - Identifies the most viewed videos per country for specific dates and months.
- **Category Processing**: Fetches category ID JSON files from the repository and normalizes them into a dataframe to count non-assignable categories per country.

## Technologies Used
- **Python 3**
- **Pandas** for Data Manipulation
- **Requests** for HTTP downloading
- **Zstandard** for `.zst` file decompression
- **Jupyter Notebook** for interactive analysis

## How to Run
1. Clone this repository to your local machine.
2. Ensure you have the required dependencies installed:
   ```bash
   pip install pandas requests zstandard
   ```
3. Open `Trending YouTube Dataset - FCS 2025-26 Project1.ipynb` in Jupyter Notebook or JupyterLab.
4. Run all cells to see the complete analysis.

## Note
This project was created as part of the FCS 2025-26 coursework.
