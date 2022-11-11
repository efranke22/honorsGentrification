# honorsGentrification
Repository for my honors statistics project at Macalester College focused on the relationship between gentrification and crime in the Twin Cities.

To replicate my analysis, please go through my files in the following steps:

Step 1: **tractData.Rmd**: In this file, I download 2010 and 2020 census data using the [tidycensus](https://walker-data.com/tidycensus/) package. 

Step 2: **tractBorderCleaning.Rmd**: In this file, I identify tracts that changed borders from 2010 to 2020. I then merge geometries as needed to create a custom set of tract borders for this analysis and calculate updated census information for these tracts. I create two final datasets which include 2010 and 2020 census information, one with all the tracts in Hennepin and Ramsey County and one with just the tracts in the Minneapolis-Saint Paul city limits.

Step 3: **definingGentrifiable.Rmd**: This is the 3rd file in my process. Here, I discuss the methods of 3 researchers in defining a "gentrifiable" census tract. I then apply these methods to the MSP tracts, denoting a tract as "gentrifiable" if at least 2/3 definitions are met. I also create a map of MSP census tracts by gentrifiable status.

Step 4: **identifyingGentrified.Rmd**: In this file I again cite 3 methods, this time for defining if a tract that has gentrified, and apply them to the MSP data. I then create a map with tract gentrification status, denoting tracts as either "Cannot gentrify", "Could but did not gentrify", and "Gentrified". I also create maps specific to each researcher's definition of gentrification.

Step 5: **crimeData.Rmd**: This is my file for downloading and cleaning the Minneapolis-Saint Paul crime data and then aggregating it with census tract gentrification information.
