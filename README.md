Netflix Data Analysis

Netflix is one of the largest streaming platforms in the world, offering thousands of movies and TV shows from various countries. The dataset used in this project contains detailed information about each title—ranging from title, director, country of origin, release year, to genre.

The objectives of this analysis are to:

Understand the distribution of content based on type (Movie/TV Show), release year, country, rating, and genre

Identify trends in content additions over time

Perform in-depth exploration of the characteristics of Movies and TV Shows on Netflix

Generate strategic insights related to global content patterns and preferences on Netflix

📌 Data Understanding & Cleaning

In the initial stage, several steps were performed to understand and prepare the data:

✔ Data Structure Check (df.info())

The dataset contains 8,807 rows and 12 columns

Several important columns are text-based, such as title, director, cast, country, and listed_in

Date-related columns such as date_added require conversion to datetime format

✔ Unique Value Inspection (df.nunique())

Initial observations include:

4,528 unique directors, indicating high creator diversity

7,692 actors involved across different titles

748 countries represented, highlighting Netflix’s global reach

17 rating categories, used for age segmentation and content regulation

✔ Handling Missing Values

Several columns contain a significant number of missing values, particularly:

director

cast

country

date_added

rating

duration

Missing values were handled using the following approach:

Category-based columns were labeled as "Unknown" to preserve distribution

date_added was converted to datetime, and missing values were not forcibly imputed

📌 Dataset Overview

The dataset consists of:

8,807 rows

12 columns

Content categorized into Movies and TV Shows

Release year range: 1925 – 2021

📌 Important Note:

This dataset does not include content released after 2021. Therefore, all trends analyzed are limited to data up to 2021. Any changes in Netflix’s strategy from 2022–2025 are not captured and should be interpreted with caution.
