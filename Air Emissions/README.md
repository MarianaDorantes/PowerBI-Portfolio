### Welcome to the Power BI Report: **Analysis of greenhouse gas emissions: emphasis on Mexico**

#### Overview: 

This report contains information on three greenhouse gases: CO2, N2O and CH4.
It is prepared for two levels of study, one is global and the other is focused only on Mexico.
The databases were obtained from open sources:
1. Historical GHG Emissions file download: https://www.climatewatchdata.org/ghg-emissions
2. Web Scraping with Python (using *pandas*) from Worldometer: https://www.worldometers.info/co2-emissions/mexico-co2-emissions/#:~:text=CO2%20emissions%20per%20capita%20in,in%20CO2%20emissions%20per%20capita.

#### Page 1: Global emissions

1. Contains 3 filters: by year, by country and by gas.
2. The cards contain the total greenhouse gas emissions and the annual global change compared to the previous year (to display a value it is necessary to select a year. Example, the user selects Year = 1997, it will give the percentage value of the difference between 1996 and 1997). This measure was created in DAX.
3. The table contains basic descriptive measures such as the minimum, average and maximum of each gas, as well as the total.
4. The historical trend for the three gases is shown.
5. The top 5 countries with the highest greenhouse gas emissions and their total are shown.
6. A heat map is shown where the concentration is indicated by a deeper shade of red.

   ![Global emissions](Global_emissions.png)


#### Page 2: Mexico's emissions 
1. Contains 3 filters: by year, by country and by sector.
2. The pie chart indicates the percentage of emissions by sector.
3. The evaluation graph was made in R, using the "corrplot" library.
4. A scatter graph of population growth and CO2 emissions is shown. The data was grouped into 4 categories using the **SWITCH** function (DAX).
5. The comparison between two data sources, their respective trend line and future projections is shown.

   ![Global emissions](Mexico_emissions.png)
