# Emergency Room Visits Dashboard

![Tableau Snapshot](https://github.com/sydflowers/Emergency-Room/blob/63c709047ed8c61a50404f10ca080c23da4b4d2d/DashboardViz.png)
(https://public.tableau.com/app/profile/sydney3387/viz/EmergencyRoom_17107900945840/Dashboard1?publish=yes)

## Purpose: 
To document creation of the Tableau Dashbaord visualization of the Emercency Room Visit data

## Data Source: 
This is from Real World Fake Data, no actual personal data was utilized for this analysis. Data can be downloaded here: https://data.world/markbradbourne/rwfd-real-world-fake-data/workspace/file?filename=Hospital+ER.csv
Note: The data contains a column called 'dmin Flag' which was not used for the analysis. 

## Process:
- Data was downloaded as csv, saved as text, and connected as a Data Source to Tableau Public
- 10 Sheets for visualizations of data were created including the static averages, Area Chart, Heatmap, and bar graphs
- For the Area Chart, a calculated field was used to break out patient ages into age ranges (0-18, 19-65 and 66+)
  The formula for the calculated field is:
  IF [Patient Age] >= 0 AND [Patient Age] <=18 THEN '0-18'
  ELSEIF [Patient Age] >=19 AND [Patient Age] <= 65 THEN '19-65'
  ELSEIF [Patient Age] >= 66 THEN '66+'
  END
- Horizontal Continers were arranged on an empty Dashboard and visualizations were dropped in from their sheets
- Inner and outer padding were adjusted to delineate areas
- Tooltips were updated to be more descriptive
- Images (Hourglass and Thumbs Up) were added above their respective line graphs
