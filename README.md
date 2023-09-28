# 2022 Tract Crosswalk
#### Census tract crosswalk to town, county, county equivalent, ZIP code, PUMA (2020), and secondary school district

The 2022tractcrosswalk.csv file contains a crosswalk between 879 Connecticut census tracts and towns, counties, country equivalents, ZIP codes, 2020 PUMAS, and secondary school districts in CT.


#### Note about FIPS Codes and County Equivalents

In 2022, the Census Bureau adopted county equivalents- Connecticut's nine planning regions- as new county-level geographies for Connecticut for statistical purposes, replacing Connecticut's eight counties in Census Bureau data products. The county equivalents have new FIPS codes. 

Census Bureau data and publications will transition to using the county equivalents instead of counties throughout 2023-2024. To help ease this transition, this crosswalk includes FIPS codes for both the counties and the new county equivalents. 

Tracts and towns therefore have two FIPS identifiers. The tract and town boundaries did not change.
- tract_fips_20 and town_fips_20 include the FIPS code from its county (county_fips_20)
- tract_fips_22 and town_fips_22 include the FIPS code from its county equivalent/planning region (ce_fips_22)


#### To prevent Excel from transforming FIPS codes and zip codes to numbers automatically (which leads to missing leading 0s), do the following:
1.	Open Excel, New workbook
2.	Go to File > Import > CSV file
3.	Choose file, and select "text" as type of tract_fips_2020, tract_fips_2022, town_fips_2020, town_fips_2022, county_fips_2020, ce_fips_2022 and zipcode columns.

Note that some tracts cross zip boundaries and some tracts cross town boundaries, this is usually the case for very small towns. Therefore, this crosswalk is approximate.

Note that tracts that contained only water and were not within municipal boundaries are excluded from this crosswalk. These are 2020 tracts 09001990000, 09007990100, 09009990000, and 09011990100.

### Sources

* 2020 TIGER/Line Shapefiles: https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.2020.html
* 2022 TIGER/Line Shapefiles: https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.2022.html
* County subdivisions (which are towns for Connecticut) on TIGER: https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2019&layergroup=County+Subdivisions
* Connecticut zipcode boundaries: https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2020&layergroup=ZIP+Code+Tabulation+Areas
* Secondary school district boundaries: http://magic.lib.uconn.edu/connecticut_data.html#education [Connecticut Secondary School Districts (rev. 5/13/2010)]

