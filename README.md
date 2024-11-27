# Project of Data Management

In our analysis of Formula 1 data from the years 2013, 2014, 2021, and 2022, we have gathered a comprehensive dataset for comparative insights.

## Data Acquisition

For each of the specified years, we meticulously collected the following data: Drivers and Teams, Grand Prix, Laps & Qualifications. We gathered detailed information on the Formula 1 qualifying sessions. We collected Maximum Speeds During Qualifying Sessions and Circuit with Turns & Length. 
Finally we meticulously documented the weather conditions during qualifying sessions and races because weather can significantly impact race outcomes and strategy.
During the data collection phase, we primarily obtained data through web scraping (BeautifulSoup and Selenium in Python), with the exception of the PDF files containing maximum speeds, which were downloaded and converted to JSON format (in Python).

## Data Quality

To verify the completeness of the acquired dataset we conducted an in-depth analysis of missing data.

We assessed data consistency by examining the update status of websites, their official sources (as in the case of the fia.com for speed data), and cross-referencing multiple sources (as in the case of weather conditions gathered from both Italian and English Wikipedia pages). 

Data accuracy was evaluated using analytical tool, the percentage of inaccuracies, and through semantic considerations. Additionally, we conducted semantic considerations, which included evaluating the reliability of data sources. In the case of weather conditions, our assessment was based on words or sentences found within the texts from which we extracted the data, and this evaluation was conducted across multiple languages to ensure consistency and accuracy.

## Data Storage

Subsequently, we integrated all the collected data from the specified years (2013, 2014, 2021, and 2022) into a consolidated dataset. 
This dataset is stored into JSON files named "Final_Datasetyear.json" on MongoDB. Once the dataset was completed, we performed three queries on the data.
