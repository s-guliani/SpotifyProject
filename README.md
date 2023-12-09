# Spotify ETL Project

[[https://images.prismic.io/soundcharts/727545d02420e55c5c6a376f633a1f02ebc59dc5_mapspot2.png?auto=compress,format]](https://www.google.com/url?sa=i&url=https%3A%2F%2Fsoundcharts.com%2Fspotify-analytics&psig=AOvVaw2YWo0Ze9G81NWCrtXb8vf7&ust=1702251853284000&source=images&cd=vfe&opi=89978449&ved=0CBIQjRxqFwoTCLD67bzEg4MDFQAAAAAdAAAAABAD)

## Overview

This project focuses on creating an ETL (Extract, Transform, Load) pipeline for Spotify data. The goal is to consolidate, transform, and store Spotify track information in a data warehouse, enabling efficient ![Uploading image.png…]()
data analysis and reporting.

## Team Members

- Sanjit Guliani

## Project Description

The project involves extracting Spotify track data, transforming it to a suitable format, and loading it into a data warehouse. This allows for in-depth analysis of track information, such as popularity, duration, and various audio features.

## Business Problem

The music industry, particularly in the streaming era, generates vast amounts of data. Analyzing this data can provide valuable insights for artists, music labels, and enthusiasts. The ETL pipeline aims to address challenges related to data consolidation, format standardization, and efficient storage for analytical purposes.

## Data

The Spotify track data is obtained from [https://research.atspotify.com/2020/09/the-million-playlist-dataset-remastered/]. It includes information on tracks, artists, albums, and various audio features.

## Methods

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
- Examples include charts depicting popularity trends, ennergy distribution, and more.



## Tools Used

- Data Storage: Amazon S3
- Data Processing: Python (Pandas, Boto3)
- Data Warehouse: Amazon Redshift
- Visualization: Tableau

## ETL Process

1. **Data Extraction:** Original data is sourced and uploaded to Amazon S3.
2. **Data Transformation:** Python scripts transform the data, addressing inconsistencies and preparing it for analysis.
3. **Data Loading:** Transformed data is loaded into Amazon Redshift for efficient storage and retrieval.

## Visualization Examples

- Price Change over time
- Share Volume over time
- Bid-Ask spread over time
- Trading Volume vs Price Change over time

## Acknowledgments

The project team would like to thank Spotify for providing access to the track data used in this analysis.

Feel free to explore the provided scripts and visualizations to gain deeper insights into the Spotify ETL project.
