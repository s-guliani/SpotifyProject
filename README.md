# Spotify ETL Project
(![spotmap](https://github.com/s-guliani/SpotifyProject/assets/145724433/cf6a2dd6-42e9-487e-a3b5-54ea10ae8cad)


## Overview

This project focuses on creating an ETL (Extract, Transform, Load) pipeline for Spotify data. The goal is to consolidate, transform, and store Spotify track information in a data warehouse, enabling efficient data analysis and reporting.

## Team Members

- Sanjit Guliani

## Project Description

The project involves extracting Spotify track data, transforming it to a suitable format, and loading it into a data warehouse. This allows for in-depth analysis of track information, such as popularity, duration, and various audio features.

## Business Problem

The music industry, particularly in the streaming era, generates vast amounts of data. Analyzing this data can provide valuable insights for artists, music labels, and enthusiasts. Real world application of this data includes but is not limited to creating music reccomendation programs, analyzing music industry trends, etc. The ETL pipeline aims to address challenges related to data consolidation, format standardization, and efficient storage for analytical purposes.

## Data

The Spotify track data is obtained from [https://research.atspotify.com/2020/09/the-million-playlist-dataset-remastered/]. It includes information on tracks, artists, albums, and various audio features.

## Methods
- Dimensional Modeling: creating a fact & dimension tables to model our data and to help us better understand the relationships between them.

<img width="501" alt="Screenshot 2023-12-09 at 6 23 10 PM" src="https://github.com/s-guliani/SpotifyProject/assets/145724433/863e4bb0-7fda-4ef9-9036-8fb0daee76fa">

### Data Extraction

- Python scripts, utilizing Boto3, are used to upload the data to Amazon S3 for storage.

### Data Transformation

- Data transformation is carried out using Python and Pandas.
- Duration is converted from milliseconds to seconds.
- Additional transformations are applied to ensure data consistency and format adherence.

### Data Loading

- Using a python script the transformed data is loaded into Amazon Redshift, a serverless data warehouse.

### Visualization

- Visualizations are created using Tableau to provide insights into Spotify track data.
- Examples include charts depicting popularity trends, ennergy distribution, song danceability, and more.

## Tools Used

- Data Storage: Amazon S3
- Data Processing: Python (Pandas, Boto3)
- Data Warehouse: Amazon Redshift
- Visualization: Tableau

## ETL Process

1. **Data Extraction:** Original data is sourced and uploaded to Amazon S3.
2. **Data Transformation:** Python scripts transform the data, addressing inconsistencies and preparing it for analysis.
3. **Data Loading:** Transformed data is loaded into Amazon Redshift for efficient storage and retrieval.
![image](https://github.com/s-guliani/SpotifyProject/assets/145724433/b19d3c9c-6b15-4a53-b22b-2e72c2f109d2)


## Visualization Examples
Song Energy trends based on Song Artists
<img width="1323" alt="Screenshot 2023-12-09 at 6 32 22 PM" src="https://github.com/s-guliani/SpotifyProject/assets/145724433/0f51e355-86a9-4e65-9e5d-c33ec4d1dad0">

Album Popularity 
<img width="1274" alt="Screenshot 2023-12-09 at 6 32 35 PM" src="https://github.com/s-guliani/SpotifyProject/assets/145724433/d0cdc4d9-88ec-40ca-81b5-6629882897eb">

Song Genre vs Danceability of a song
<img width="1274" alt="Screenshot 2023-12-09 at 6 32 44 PM" src="https://github.com/s-guliani/SpotifyProject/assets/145724433/adc080a2-34a4-460f-9c88-01ade069f141">

Song Popularity 
<img width="1274" alt="Screenshot 2023-12-09 at 6 32 52 PM" src="https://github.com/s-guliani/SpotifyProject/assets/145724433/e7ef1c5e-dd17-4843-9f81-28aa956cf956">
