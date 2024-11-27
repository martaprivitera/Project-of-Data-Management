# Project of Data Management

This repository contains different sub-folders in which we can find all the codes and JSON files created. A brief
explanation of the contents:

1. The WebScraping codes can be found in the “Data Acquisition” folder, in particular we have to make
reference to 3 sub-folders:

- “Seasons”, which contains the four python codes about each year;

- “Qualifying Max Speed, which contains four folders with the pdf we downloaded for eache year
and then the python codes of conversion from pdf to JSON for each year;

- “Weather”, which contains two folders, one for the Qualifying session and the other for the Race
where we can find the python code for each year.

2. The output of these WebScraping can be found in the “RawDataCollected” folder which contains the
“WebScraping” folder in which the JSON output relative to Season, Max Speed and Weather Conditions
are collected (divided by sub-folders).

3. In the “Data Acquisition” folder we can also find the codes relative to the merge between Season JSON,
Maximum Speed JSON and Weather Conditions JSON. In particular they are contained in the “Merge”
folder. The outputs of the merge process are contained in the “Merged Data” folder in which there
are the integration between Season JSONs and Maximum Speed JSONs. The JSONs with the last
integration plus Weather Condition are stored in the “Final Data” folder;

4. The “Data quality” folder contains several codes and JSON files:

- The ones to check data quality on season JSON (rawdata seasons.py which has as output the
laps2013.JSON, laps2014.JSON, laps2021.JSON and laps2022.JSON ), Max Speed JSON (raw-
data speed.py) and Weather Condition JSON (rawdata weather.py);

- The four python codes for doing WebScraping (e.g laps2013fia.py) on the FIA website with re-
spective outputs (e.g laps2013fia.JSON ) and the code that checks correspondences between FIA
website and our JSON files (lapscheckfia.py);

- The two python codes about the data quality check on merged data (merge speed.py and merge weather.py);

- The python code for data quality on stored data (finaldata.py)

5. Finally, the “Data Storage” folder contains:
 
- The python codes that make connection and insertion of the final JSON files to MongoDB;

- The 3 query codes we used for our analysis and another code to plot useful graphs we used and
inserted in the Report (DataM anagementReport.pdf).
