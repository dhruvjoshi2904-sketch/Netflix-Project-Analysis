# Netflix Global Expansion Strategy — Data Analysis Project

## Project Overview

This project explores Netflix's content distribution across countries and examines where further market research may be useful.

**Challenge:** Global Expansion Strategy  
**Main business question:** Which countries contribute the most content to Netflix, and where could Netflix expand next?

The analysis uses Python in a Jupyter Notebook to clean and explore the catalogue data, compare Movies and TV Shows, examine content additions over time, and develop business insights and recommendations.

## Team Members and Roles

| Team Member | Student Email | Division | Role |
|---|---|---|---|
| Bhavik Devani | 00101399@students.schiller.edu | Division A | Project Manager |
| Aksh Patel | 00101831@students.schiller.edu | Division A | Exploratory Data Analysis (EDA) |
| Nisarg Padia | 00102650@students.schiller.edu | Division B | Data Collection |
| Shweta Ajudeeya | 00102792@students.schiller.edu | Division B | Data Visualization |

## Project Files

Keep the following two files in the same folder:

- `Netflix_Global_Expansion_Challenge2_Full(3).ipynb` — Jupyter Notebook containing the analysis.
- `netflix_global_expansion_synthetic(2).csv` — CSV file used by the notebook.

> **Important:** The supplied CSV is a synthetic, Netflix-style dataset for this project. The findings describe this dataset and should not be interpreted as official Netflix business figures.

## Dataset Description

The dataset contains **924 rows and 12 columns** before cleaning.

| Column | Description |
|---|---|
| `show_id` | Unique identifier assigned to a title |
| `type` | Content type: Movie or TV Show |
| `title` | Title name |
| `director` | Director name |
| `cast` | Cast members |
| `country` | Country or countries associated with the title |
| `date_added` | Date the title was added to the catalogue |
| `release_year` | Original release year |
| `rating` | Content age rating |
| `duration` | Movie duration or number of TV show seasons |
| `listed_in` | Genre or category |
| `description` | Short title description |

## Tools and Libraries

- Python
- Jupyter Notebook
- pandas — data loading, cleaning, and analysis
- NumPy — numerical and data operations
- Matplotlib — charts and visualizations
- Seaborn — statistical visualizations

## Analysis Workflow

1. Import the required Python libraries.
2. Load the CSV dataset and inspect its structure.
3. Review data types, missing values, summary statistics, and duplicate rows.
4. Remove exact duplicate rows and standardize text fields.
5. Convert date and numeric columns to appropriate data types.
6. Handle missing country values by labelling them as `Unknown`.
7. Split multi-country entries so each title-country relationship can be analysed separately.
8. Perform exploratory data analysis.
9. Create visualizations to compare content types, countries, and catalogue additions over time.
10. Summarize business insights, recommendations, and the final conclusion.

## Key Findings

After removing exact duplicate rows, the dataset contains **901 rows** and **900 distinct title IDs**.

- Movies: **615**
- TV Shows: **286**
- Countries represented in the known country records: **24**
- Top country contributions:
  1. United States — **222**
  2. India — **111**
  3. United Kingdom — **92**
  4. South Korea — **65**
  5. Japan — **61**

A title associated with more than one country is counted once for each country in the country-level analysis. Therefore, country contribution counts represent title-country associations and do not add up to the total number of titles.

## Business Insights and Recommendations

The analysis identifies the United States, India, and the United Kingdom as the largest contributors in the dataset. Movies are more numerous than TV Shows. India, South Korea, and Japan also have notable content contributions.

The project recommends:

- Continuing to study content performance in countries with high catalogue contributions.
- Exploring regional and local-language content preferences.
- Researching countries with lower catalogue representation before considering expansion.
- Reviewing the balance between Movies and TV Shows.
- Using audience demand, viewing behaviour, subscriptions, costs, licensing, and competition data before making actual market-entry decisions.

Lower content representation alone does not prove that a country is a good expansion opportunity.

## How to Run the Project

1. Download the Jupyter Notebook and CSV file.
2. Save both files in the same folder.
3. Open Jupyter Notebook or JupyterLab.
4. Open `Netflix_Global_Expansion_Challenge2_Full(3).ipynb`.
5. Run the notebook cells from top to bottom.

If you use Google Colab, upload the CSV file and update the notebook's `DATA_PATH` if the file is not in the notebook's current working directory.

## Expected Output

When the notebook runs successfully, it displays:

- Dataset previews and data-quality checks
- Cleaned dataset information
- Movie and TV Show counts
- Top 10 countries by title contribution
- Country-level Movies vs TV Shows comparison
- Catalogue additions over time for the leading countries
- Release-year distribution
- Country screening table
- Business insights, recommendations, and final conclusion

## Conclusion

This project demonstrates how data cleaning, exploratory data analysis, and visualization can help identify content distribution patterns and potential areas for further market research. The results provide a starting point for strategic discussion; reliable expansion decisions would require real audience, financial, and market data.
