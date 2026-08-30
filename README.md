# Netflix Movies and TV Shows – Data Visualization & Storytelling

## Project Overview

This project was completed as part of the Data Analyst Internship.

The objective of this project is to clean, analyze, visualize, and communicate
insights from a Netflix Movies and TV Shows dataset using Python and Microsoft Power BI.

The project focuses on data visualization and storytelling by creating an
interactive Power BI dashboard that presents key insights about Netflix content.



##  Objectives

- Clean and prepare the raw Netflix dataset.
- Handle missing and incorrect values.
- Standardize text values and column names.
- Remove duplicate records.
- Perform basic data analysis.
- Create meaningful visualizations using Power BI.
- Build an interactive dashboard.
- Present insights through data storytelling.
- Highlight important business insights from the dataset.



## Tools & Technologies

- Python
- Pandas
- NumPy
- Jupyter Notebook
- Microsoft Power BI
- Power Query
- DAX
- Git & GitHub



##  Dataset

The dataset contains information about Netflix movies and TV shows.

## Main Columns

- `show_id`
- `type`
- `title`
- `director`
- `cast`
- `country`
- `date_added`
- `release_year`
- `rating`
- `duration`
- `listed_in`
- `description`



#  Data Cleaning

The raw dataset was cleaned using Python and Pandas.

### Data cleaning steps performed:

1. Loaded the raw CSV dataset.
2. Standardized column headers:
   - Removed leading/trailing spaces.
   - Converted column names to lowercase.
   - Replaced spaces with underscores.
3. Checked missing values.
4. Handled missing values in text/categorical columns.
5. Corrected incorrect values in the `rating` column.
6. Moved incorrect duration values such as:
   - `66 min`
   - `74 min`
   - `84 min`
   
   from the `rating` column to the `duration` column.
7. Standardized text values.
8. Removed extra spaces.
9. Standardized the `type`, `country`, `rating`, and `show_id` fields.
10. Corrected data types.
11. Checked and removed duplicate rows.
12. Performed a final data quality check.
13. Saved the cleaned dataset as:

`netflix_titles_CLEANED.csv`


#  Data Visualization

The cleaned dataset was imported into Microsoft Power BI to create an
interactive Netflix Content Analysis dashboard.

The dashboard follows data visualization best practices by selecting
appropriate charts, avoiding unnecessary visual clutter, highlighting
important findings, and focusing on insights rather than visuals alone.



#  Power BI Dashboard

## KPI Cards

The dashboard contains four KPI cards:

- Total Titles
- Total Movies
- Total TV Shows
- Movie %

These provide a quick overview of the Netflix content catalog.



##  Visualizations

### 1. Netflix Content by Type

**Chart:** Donut Chart

Shows the distribution of:

- Movies
- TV Shows

This visualization helps understand the overall composition of the Netflix
content catalog.


### 2. Netflix Content Added Over Time

**Chart:** Line Chart

Shows the number of Netflix titles added over different years.

This helps identify growth patterns and periods when Netflix added a large
amount of content.



### 3. Top Countries by Number of Titles

**Chart:** Horizontal Bar Chart

Displays the top countries based on the number of titles.

The chart makes it easier to compare content contribution across countries.



### 4. Netflix Titles by Rating

**Chart:** Horizontal Bar Chart

Shows the distribution of Netflix titles across different content ratings.

This provides an understanding of the types of content available for
different audience categories.



### 5. Netflix Titles by Release Year

**Chart:** Column Chart

Shows the number of titles based on their release year.

This helps identify the distribution of older and newer content in the dataset.


### 6. Movies vs TV Shows Added Over Time

**Chart:** Stacked Column Chart

Compares Movies and TV Shows added to Netflix over time.

This visualization helps understand how the content mix changed across the
years.


#  Interactive Filters

The Power BI dashboard includes interactive filters/slicers for:

- Content Type
- Rating
- Year Added

These allow users to explore the dataset dynamically and analyze specific
segments of Netflix content.



#  Key Insights

### 1. Movies dominate the catalog

Movies represent the majority of titles in the Netflix dataset, while TV
Shows make up a smaller portion of the catalog.

### 2. Netflix content additions increased significantly

The number of titles added to Netflix increased considerably during the later
years represented in the dataset.

### 3. United States has the largest content contribution

The United States has the highest number of titles among the countries shown
in the dashboard.

### 4. TV-MA is a major rating category

TV-MA represents the largest rating category in the dashboard, indicating a
large amount of mature-audience content.

### 5. Content growth varies by year

The release-year visualization shows that the Netflix catalog contains a
large concentration of titles from more recent years.



#  Data Storytelling

The dashboard presents the analysis as a story:

**1. What is in the Netflix catalog?**

The KPI cards and content-type donut chart provide an overview of the total
content and the Movie/TV Show distribution.

**2. How has Netflix content grown?**

The line chart shows how the number of titles added changed over time.

**3. Where does the content come from?**

The country chart highlights the major countries contributing content.

**4. What type of content is available?**

The rating chart provides an overview of the content rating distribution.

**5. How has the content mix changed?**

The stacked column chart compares Movies and TV Shows added over time.



#  Project Structure

```text
Netflix-Movies-and-TV-Shows/
│
├── Dataset/
│   ├── netflix_titles_RAW.csv
│   └── netflix_titles_CLEANED.csv
│
├── Data_Cleaning/
│   └── Netflix_Data_Cleaning.ipynb
│
├── PowerBI/
│   └── Netflix_Data_Visualization.pbix
│
├── Screenshots/
│   └── Netflix Movies and Tv Shows Dashboard.png
│
└── README.md
