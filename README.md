# Premier-League-Team-Performance-Analysis
This repository utilizes excel, power query and power pivot to analyze premier league data for the season 2020,2021,2022,2023 and 2024.

# The Data
- The dataset for this project is obtained from Kaggle [here](https://www.kaggle.com/datasets/sajkazmi/premier-league-matches). It containes data from the premier league for the seasons 2020 to 2024. The dataset has key features including the teams, the matchdays,the captains, the referees, the date and time among other features. The raw data contains `4,789 rows` and `27 Columns`. 

# Tools
- Power Query
- Excel
- Power Pivot

   **Power Query**:
  - We utilize this to perform ETL(Extract Transform and Load). The dataset is loaded into power query first.
  - In power query, convert the columns into the correct data types, remove any duplicates, delete any unwanted columns and crete any calculated columns or custom columns as required.
  - In this dataset, I split the date column into 2 to allow for UK time and Central European Time. I changed the data types to date using locale. I rearranged the columns to ensure there is flow when reading the data. I created a calculated columns to show whether there is a home or away win or lose including a draw.I deleted the matchreport column since its unecessary and renamed most columns to ensure I can best be able to explore the data.
  - Ensure that there are no duplicates, the team names are consistent by replacing with one consistent name on power Query. For example replace `West Brom` with `West Bromwich Albion` to have one consistent name for the respective team.

    **Power Pivot**:
    - This is to enable data modeling using DAX(Data Analysis Expressions). It allows for complex metrics.
    - In power Pivot, create calculated columns like Goals For, Goals Against, Goal difference, Points, matches played, wins and draws.
    - From powe pivot insert a pivot table and use a timeline to show the premier league standing for each season.
