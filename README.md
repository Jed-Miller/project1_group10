# The Effect of Snowpack in the Central Sierras  Counties on Wildfire Severity in Outlying Counties

A project for UCB Extension, written and analyzed by:

Estelle Santini, Kyle Stephens, Karina Quintana, Borna Karimi, Jed Miller, and Jake Pohs

### **Description**

An analysis on the effect of winter snowpack on the severity of wildfires in the Central Sierras based on wildfire data from the California Department of Forestry and Fire Prevention and snow data from the California Department of Water Resources.

### Data Sources

| Name                                                  | Type | Description                                                                                                                                                                                                                                                                | Website                                           |
| ----------------------------------------------------- | ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------- |
| CDEC California Department of Water Resources         | JSON | API that provides daily snowpack data for a ten year period                                                                                                                                                                                                                | https://cdec.water.ca.gov/dynamicapp/wsSensorData |
| California Department of Forestry and Fire Prevention | CSV  | "Incident data is provided in raw, computer readable formats and requires further processing using specialized software. Two additional API parameters include year (values include a year in the YYYY format) and inactive (values include true and false)." Per website. | https://www.fire.ca.gov/incidents/                |

### Introduction

Put intro here

### Hypothesis

H `<sub>`0 `</sub>`: Snowpack depth in the central Sierras has no effect on wildfire severity: number of fires, acreage burned, or duration of burns in the outlying counties.

H`<sub>`a1`</sub>`: Increased snowpack depth in the central Sierras will decrease the number of fires in the outlying counties in the corresponding fire season.

H`<sub>`a2`</sub>`: Increased snowpack depth in the central Sierras will decrease the amount of acres burned in the outlying counties in the corresponding fire season.

H`<sub>`a3`</sub>`: Increased snowpack depth in the central Sierras will decrease the duration of wildfire burn in the outlying counties in the corresponding fire season.

### Data

We used the data provided by the California State government for our analysis. The snowpack data was sourced through an API from the California department of Water Resources. Our fire data was a CSV provided by the California Department of Forestry and Fire Protection. Each dataset was check for data authentication before being imported to pandas

The data we imported was from the previous 10 years. We examined and cleaned the data sets separately. This was due to the winter season spanning two years for any fire season following after. We had to arrange this snowpack data to include the data from the year previous to the fire season. Once the winter months were organized we were able to structure our data with a column for Winter 12/13 and Fire Season 2013.

Calculations for average, median, max, and min were performed to analyze the datasets further and graphs were created to show our findings.

### Analysis

Put analysis here

### Conclusion

Put conclusion here
