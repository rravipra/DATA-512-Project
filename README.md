# DATA-512-Project

Link to the reflection doc: https://docs.google.com/document/d/1ePp23lR5Txo646iXEQiWodc_BTwDIUuTXuEkLR6bTD4/edit?usp=sharing

# PART 1:

# Goal:

The goal of the part 1 of this project is to answer the research question: what are the estimated smoke impacts on your assigned city for the last 60 years? by creating an annual estimate of wildfire smoke in a city that I am interested in which is Helena, Montana in my case:

The goal is to create an annual estimate of wildfire smoke in Helena, Monatana. This estimate is just a number that you can eventually use to build a predictive model. Technically, smoke impact should probably be considered the health, tourism, economic or other social problems that result from the smoke. For this we'll generically call your estimate the wildfire smoke impact. We need some kind of number to represent an estimate of the smoke your city saw during each annual fire season.

The smoke estimate adheres to the following conditions:
1. The estimate only considers the last 60 years of wildland fires (1963-2023).
2. The estimate only considers fires that are within 1250 miles of your assigned city.
3. An annual fire season will run from May 1st through October 31st.

# Data:

Wildfire dataset: https://www.sciencebase.gov/catalog/item/61aa537dd34eb622f699df81

Example notebooks epa_air_quality_history_example.ipynb and wildfire_geo_proximity_example.ipynblicensed by: [Creative Commons](https://creativecommons.org) [CC-BY license](https://creativecommons.org/licenses/by/4.0/)

Air Quality System (AQS) API: [Documentation](https://aqs.epa.gov/aqsweb/documents/data_api.html)

Additional information on AQS: [here](https://www.epa.gov/outdoor-air-quality-data/frequent-questions-about-airdata)

# Code files:

The notebooks file in this repository are:

- Calculate_smoke_impact.ipynb
- Calculate_AQI_estimate.ipynb

(These below two code example was developed by Dr. David W. McDonald for use in DATA 512, a course in the UW MS Data Science degree program. This code is provided under the [Creative Commons](https://creativecommons.org) [CC-BY license](https://creativecommons.org/licenses/by/4.0/). Revision 1.0 - August 13, 2023
- epa_air_quality_history_example.ipynb
- wildfire_geo_proximity_example.ipynb
- wildfire.zip

# Data Files created from the code:

1) academy_monthly_desktop_20150101-20230401.json
2) academy_monthly_mobile_20150101-20230401.json
3) academy_monthly_cumulative_20150101-20230401.json

All of these can be found in the JSON_files.rar folder from where you can extract it from.

**Structure of the JSON files:**

For the smoke impact estimation

**Key**: Years

**Value**: A list of estimate values.

For the AQI estimation:

**Key**: Years

**Value**: AQI estimates:

# Images of graphs acquired from the code outputs:

The code also outputs many graphs which is present and is mentioned in detail in the google doc file like [here](https://docs.google.com/document/d/1ePp23lR5Txo646iXEQiWodc_BTwDIUuTXuEkLR6bTD4/edit?usp=sharing):

Time series prediction for the next 25 years based on the smoke impact estimate:

![image](https://github.com/rravipra/DATA-512-Project/assets/46725716/596f593d-fc8f-41a8-b34f-36fc6b26668a)

# Considerations with the Data:

- It is important to note that the when it comes to calculating the smoke impact estimates for each of the years, in my case I did not have the data for the years 2021, 2022, and 2023 so my estiamtes was only from 1963-2020.
- Even in the data to get the AQI scores while getting the Gaseous AQI pollutants and the Particulate AQI pollutants it is not necessary that the data for both are present for all the years. I only found data for both from 1986-2023 which I have used.


