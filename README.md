# Premier-League-Team-Performance-Analysis
This repository utilizes excel, power query and power pivot to analyze premier league data for the season 2020,2021,2022,2023 and 2024 with a specific focus on Liverpool Football Club vs Mnchester City.

# The Data
- The dataset for this project is obtained from Kaggle [here](https://www.kaggle.com/datasets/sajkazmi/premier-league-matches). It contains data from the premier league for the seasons 2020 to 2024. The dataset has key features including the teams, the matchdays,the captains, the referees, the date and time among other features. The raw data contains `4,789 rows` and `27 Columns`. 

# Tools
- Power Query
- Excel
- Power Pivot

  **Power Query**:
   - We utilize this to perform ETL(Extract Transform and Load). The dataset is loaded into power query first.
   - In power query, convert the columns into the correct data types, remove any duplicates, delete any unwanted columns and create any calculated columns or custom columns as required.
   - In this dataset, I split the date column into 2 to allow for UK time and Central European Time. I changed the data types to date using locale. I rearranged the columns to ensure there is flow when reading the data. I created a calculated columns to show whether there is a home or away win or lose including a draw.I deleted the matchreport column since its unecessary and renamed most columns to ensure I can best be able to explore the data.
   - I ensured that there are no duplicates, the team names are consistent by replacing with one consistent name on power Query. For example replace `West Brom` with `West Bromwich Albion` to have one consistent name for the respective team.
   - Finally I loaded the dataset on excel.

  **Power Pivot**:
    - This is to enable data modeling using DAX(Data Analysis Expressions). It allows for complex metrics.
    - From Excel, I added the loaded power query table to the data model on power pivot.
    - In power Pivot, create calculated columns like Goals For, Goals Against, Goal difference, Points, matches played, wins and draws.
    - From power pivot insert a pivot table and use a timeline to show the premier league standings for each season. Compute the winrate measure as well on power pivot.
    - From power pivot, insert desired charts to visualize the data set.

  **Excel**:
  - From excel, we build interactive pivot tables with slicers and filters to better interact with the data.
  - Each sheet is used to communicate information on the performance of teams and how they compare with special focus on Liverpool and manchester City, using the filters, comparisons can be made of other teams of interest.
  - A final dashbooard that presents everything on one page is prepared on the first worksheet.
 
 # Key Findings
- On Average, Liverpool had a win rate of 64.74% compared to Manchester City's 72.63%.
- Liverpool drew many matches '40' compared to City's '26'. Interstingly, Liverpool only lost one more match '27' than City '26'. It can be concluded that Liverpool's performance could generally improve if they could eliminate or reduce the number of draws per season.
- In the season 2022, where City defeated Liverpool to the championship by a single point, Liverpool had 8 draws compared to City's 6. If Liverpool had won just one of those matches, they would have been champions.
- Looking at the points tally, Manchester City is a far more consistent team which perphaps is the reason why they were champions foru years in a row.


 # Files
- [The Complete Excel File](Premier_League_Team_Performance_Analysis_Complete.xlsx)
- [Visuals](Visualizations)
- [Dashboard](Premier_League_Team_Performance_Analysis_Dashboard.pdf)

 # How to run
 - Download the dataset from [here](PremierLeague20202024rawdata.csv)
 - Download the Complete Excel File and recreate the power query, power pivot and charts operations.
 - View the Dashboard and recreate it.
 
