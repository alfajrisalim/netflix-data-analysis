## Netflix Data Analysis

Netflix is one of the largest streaming platforms in the world, offering thousands of movies and TV shows from various countries. The dataset used in this project contains detailed information about each title—ranging from title, director, country of origin, release year, to genre.

The objectives of this analysis are to:

Understand the distribution of content based on type (Movie/TV Show), release year, country, rating, and genre

Identify trends in content additions over time

Perform in-depth exploration of the characteristics of Movies and TV Shows on Netflix

Generate strategic insights related to global content patterns and preferences on Netflix

## Key Insights

- **Movies dominate the catalog (~70%)**, significantly exceeding TV Shows.
- **Content additions increased substantially between 2015–2019**, reflecting Netflix's rapid content expansion during this period.
- **The United States and India are the largest content contributors**, highlighting the importance of these markets in Netflix's global catalog.
- **Drama and International Movies are among the dominant genres**, reflecting Netflix's broad international content strategy.
- **Missing country information is present in the dataset**, indicating limitations in metadata completeness, particularly for older content.

## Conclusion

The analysis shows that Netflix's catalog is dominated by Movies and internationally oriented content, with Drama and International Movies representing major genre categories. Content additions increased substantially during 2015–2019, while the United States and India emerged as the largest content contributors.

The catalog also shows substantial diversity across genres, ratings, actors, and directors. Adult-oriented ratings such as TV-MA and TV-14 are prominent, while children's content represents a smaller segment of the catalog.

Overall, the analysis provides an overview of Netflix's content composition, geographic distribution, genre preferences, and content acquisition trends over time.

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
