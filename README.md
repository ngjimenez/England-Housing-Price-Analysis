# Understanding the English Region / Areas
The Area Codes are defined by the Office for National Statistics (ONS) and reflect the hierarchy of government in the UK. We have simplified the data so it is not necessary to
understand the full ONS codes, but if you want to understand the full details read https://en.wikipedia.org/wiki/ONS_coding_system.

In the provided data:
  * Each area of the country is covered twice, at different levels.
  * Level 1 is a region. There are 9 regions in England (examples are ‘London’, ‘South East’, ‘South West’).
  * Level 2 is a local government area. There are 4 different types of local government areas, though the distinction is not important in our analysis. Each area belongs to
one of the regions.

#### Relationship Between Area and Region
A separate file location-codes.csv shows which region each area belongs to. Note
that here is some overlap between the two files, such as the names of the areas and
regions. This file can be used to determine which of the 9 regions each area is in.

# Analysis Goals

The analysis is done in four parts. 
* Part 1: Load and prepare the data
As described above, the data file includes both data for areas and for regions. Both region data and area data are needed below, but they need to be separated 
(into separate data frames).
  * Separate the region data (with ‘E12’ prefix codes) from the area data (other prefixes).
  * Use the ‘location code’ data file to add to each area price record the region to which the area belongs, ensuring that all areas have been assigned a region.
  * Check the data for missing values in the region or area data; decide how to act, giving a clearly description and justification.

* Part 2: Trends
Use the region data in this section to look at some trends.
  * Plot trends of the prices, considering only flats and detached properties. The plots should cover the prices in the 9 regions over the 36 months.
  * Choose a number / variety of plots so that the trends can be easily understood and compared.
  * Comment on the trends. Compare the regions, the two property types and different times of year.


* Part 3: Price Changes
Use the area data in this section to look at how flat prices have changed.
  * Calculate the change in the price of flats in each area between July 2017 and July 2018.
  * Choose a way (or ways) to visualise the change in area prices in each region.
  * Comment on the results, describing any patterns that you see.

* Part 4: Statistical Analysis
Use the area data in this section and the work (section 2.3) on price changes to investigate
whether there is evidence that the change in the price of flats has affected all the regions
similarly.
  * Cross-tabulate the number of areas in which the price has increased and the number has decreased, by region
  * Use a chi-square test to determine whether there is evidence that the regions differ.
  * Interpret the results you obtain, including what you can and cannot determine from the result.
