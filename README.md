# Netflix Data Analysis Project

This project involves analyzing the Netflix Movies and TV Shows dataset using Python (Pandas, Seaborn) and Power BI. The goal is to extract insights, perform data cleaning, and visualize trends related to content on Netflix.

## Project Structure

- **Netflix_python.ipynb**: A Jupyter Notebook containing the Python code for data cleaning, exploration, and analysis.
- **NetFlix_Dashboard.pbix**: A Power BI dashboard visualizing key metrics and trends from the dataset.
- **netflix_titles.csv**: The source dataset containing information about movies and TV shows on Netflix.

## Technologies Used

- **Python**: For data manipulation and analysis.
    - **Pandas**: Dataframe manipulation, filtering, and aggregation.
    - **Seaborn/Matplotlib**: Data visualization (Heatmaps, Bar graphs).
- **Power BI**: For interactive dashboard creation.

## Dataset

The dataset used (`netflix_titles.csv`) contains the following key attributes:
- **Show Id**: Unique ID for every Movie / TV Show.
- **Type**: Identifier - A Movie or TV Show.
- **Title**: Title of the Movie / TV Show.
- **Director**: Director of the Movie / TV Show.
- **Cast**: Actors involved in the movie / show.
- **Country**: Country where the movie / show was produced.
- **Date Added**: Date it was added on Netflix.
- **Release Year**: Actual Release year of the movie / show.
- **Rating**: TV Rating of the movie / show.
- **Duration**: Total Duration - in minutes or number of seasons.
- **Listed In**: Genre.
- **Description**: The summary description.

## Key Analyses & Insights

The Python analysis covers the following 14 problem statements:

1.  **Duplicate Records**: Identified and removed duplicate data records.
2.  **Null Value Handling**: Visualized missing values using heatmaps.
3.  **Specific Content Info**: Retrieved details like Show ID and Director for specific titles (e.g., 'House of Cards').
4.  **Release Year Trends**: Analyzed the year with the highest number of releases using bar graphs.
5.  **Content Type Distribution**: Compared the count of Movies vs. TV Shows.
6.  **Year-wise Filtering**: Filtered movies released in specific years (e.g., year 2000).
7.  **Regional Content**: Identified TV Shows released exclusively in India.
8.  **Top Contributors**: Listed the top 10 directors with the most content on Netflix.
9.  **Genre & Region Filtering**: Filtered content based on specific criteria like 'Comedies' or 'United Kingdom'.
10. **Cast Analysis**: Counted appearances of specific actors (e.g., Tom Cruise).
11. **Rating Insights**: Explored unique ratings and filtered content based on rating, type, and country (e.g., 'TV-14' in Canada).
12. **Duration**: Determined the maximum duration of movies/shows.
13. **Country-wise Stats**: Identified the country with the highest number of TV Shows.
14. **Sorting**: Sorted the dataset by release year (Newest to Oldest).

## Power BI Data Transformation

To optimize the dataset for visualization in Power BI, the following column transformations were applied (mirroring the Python analysis steps):

- **Date Conversion**: The `date_added` column was converted to a standard format (`date_n`) to enable year-wise analysis and filtering.
- **Duration Handling**: The `duration` column was split into numeric `minutes` and string `unit` columns to allow for calculation of maximum duration and accurate time-based comparisons.
- **Data Cleaning**: Rows with missing critical values were likely handled or dropped to ensure dashboard accuracy.

## How to Run

### Python Analysis
1.  Ensure you have Python installed with the following libraries:
    ```bash
    pip install pandas seaborn matplotlib
    ```
2.  Open `Netflix_python.ipynb` in Jupyter Notebook or VS Code to view and run the analysis.

### Power BI Dashboard
1.  Install Microsoft Power BI Desktop.
2.  Open the `NetFlix_Dashboard.pbix` file to explore the interactive visualizations.
