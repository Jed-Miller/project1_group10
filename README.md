# The Effect of Snowpack in the Central Sierras on Wildfire Severity in Outlying Counties

A project for UCB Extension, written and analyzed by:

Estelle Santini, Kyle Stephens, Karina Quintana, Borna Karimi, Jed Miller, and Jake Pohs

### **Description**

An analysis on the effect of winter snowpack on the severity of wildfires in the Central Sierras based on wildfire data from the California Department of Forestry and Fire Prevention and snow data from the California Department of Water Resources.

### Data Sources

| Name                                                  | Type | Description                                                                                                                                                                                                                                                                | Website                                           |
| ----------------------------------------------------- | ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------- |
| CDEC California Department of Water Resources         | JSON | API that provides daily snowpack data for a ten year period                                                                                                                                                                                                                | https://cdec.water.ca.gov/dynamicapp/wsSensorData |
| California Department of Forestry and Fire Prevention | CSV  | "Incident data is provided in raw, computer readable formats and requires further processing using specialized software. Two additional API parameters include year (values include a year in the YYYY format) and inactive (values include true and false)." Per website. | https://www.fire.ca.gov/incidents/                |

### Hypothesis

H <sub>0</sub>: Snowpack depth in the central Sierras has no effect on wildfire severity: number of fires, acreage burned, or duration of burns in the outlying counties.

H <sub>a1</sub>: Increased snowpack depth in the central Sierras will decrease the number of fires in the outlying counties in the corresponding fire season.

H <sub>a2</sub>: Increased snowpack depth in the central Sierras will decrease the amount of acres burned in the outlying counties in the corresponding fire season.

H <sub>a3</sub>: Increased snowpack depth in the central Sierras will decrease the duration of wildfire burn in the outlying counties in the corresponding fire season.

### Data

We used the data provided by the California State government for our analysis. The snowpack data was sourced through an API from the California department of Water Resources. Our fire data was a CSV provided by the California Department of Forestry and Fire Protection. Each dataset was checked for data authentication before being imported to pandas

The data we imported was from the previous 10 years. We examined and cleaned the data sets separately. This was due to the winter season spanning two years for any fire season following after. We had to arrange this snowpack data to include the data from the year previous to the fire season. Once the winter months were organized we were able to structure our data with a column for Winter 12/13 and Fire Season 2013.

Calculations for average, median, max, and min were performed to analyze the datasets further and graphs were created to show our findings.

### Analysis

### Annual Fire Analysis


![Annual Fires in Central Sierras](./figures/annual_depth_fire_count_line.png "Annual Fire Line (Corresponding)")

![Annual Fires in Central Sierras](./figures/bar1.png "Annual Fire Bar (Corresponding)")

![Annual Fires in Central Sierras](./figures/scatter1.png "Annual Fire Scatter (Corresponding)")

![Annual Fires in Central Sierras](./figures/scatter2.png "Annual Fire Bar (Following)")

![Annual Fires in Central Sierras](./figures/bar2.png "Annual Fire Scatter (Following)")

### Avg. Acres Burned Analysis

![Annual Fires in Central Sierras](./figures/current_year_acres_burned.png "Avg. Acres Burned (Corresponding)")

![Annual Fires in Central Sierras](./figures/scatter_mean_depth_mean_acres.png "Scatter  Avg.Acres Burned (Corresponding)")

![Annual Fires in Central Sierras](./figures/following_year_acres_burned.png "Avg. Acres Burned (Following)")

![Annual Fires in Central Sierras](./figures/scatter_following_mean_depth_mean_acres.png "Scatter Avg. Acres Burned (Following)")

### Avg. Fire Duration by County Analysis

![Annual Fires in Central Sierras](./figures/avg_fire_duration_county.png "Line Avg. Fire Duration (Corresponding)")

![Annual Fires in Central Sierras](./figures/2015_corresponding_bargraph.png "Bar Avg. Fire Duration 2015 (Corresponding)")

![Annual Fires in Central Sierras](./figures/2019_corresponding_bargraph.png "Bar Avg. Fire Duration 2019 (Corresponding)")

![Annual Fires in Central Sierras](./figures/2015_following_bargraph.png "Bar Avg. Fire Duration 2015 (Following-2016)")

![Annual Fires in Central Sierras](./figures/2019_following_bargraph.png "Bar Avg. Fire Duration 2019 (Following-2020)")

Through our analysis we examined the hypotheses and created graphs to help us interpret the data. We found that having a higher average level of snowpack over the winter had a statistically significant correlation with a reduced frequency of wildfires in the following summer. In addition, we also found an inverse effect between the ammount of snowpack and the number of acres burned in the following summer; higher snowpack seemed to lead to more acres burned. However these findings were not statistically signinficant. Our analysis also showed that in years with higher snowpack, forest fires had shorter durations.

Further details of our analysis can be found in our google slides presentation: https://docs.google.com/presentation/d/1KDKdwDSVYIK-MHqCqFfhZmxBYS87GnyUiEdqaOnU4bM/edit#slide=id.p

### Conclusion

Snowpack measures directly impact the effects of the following and corresponding fire seasons. The correlations were generally not strong but the null hypothesis could not be proven.

Snowpack measures directly correlated with severity of fires in the following season, likely because of a growth of vegetation from the large snowpack from the previous year.
