# Texas Power Crisis
By [Carmen Hoyt](https://ceh58.github.io/) [@ceh58](https://github.com/ceh58)

## About
In February of 2021, Texas experienced a series of extreme winter storms that exposed vulnerabilities in the power grid. The resulting power outages disproportionately affected different socioeconomic groups in Houston, Texas. Using 4 different datasets (VIIRS, roads, houses, and socioeconomic data), this analysis investigates the impacts of these power outages on the residents of the Houston metropolitan area, particularly the distribution of outages relative to median household income.

## Skills
This analysis harnesses the following valuable skills:

- Reclassifying rasters
- Masking rasters
- Vectorizing rasters
- Transforming Coordinate Reference Systems
- Buffering features
- Mapping with `tmap`

The `stars` and `terra` packages were useful for working with raster data, and the `sf` package was used for working with vector data. 

## Repository Structure
```
├── .gitignore
├── README.md
├── texas_power_crisis.Rproj
├── texas_power_crisis.html # Rendered document
└── texas_power_crisis.qmd # Quarto document detailing the analysis
```
## Data Access

All the data used in this analysis was downloaded from a pre-prepared [Google Drive](https://drive.google.com/file/d/1bTk62xwOzBqWmmT791SbYbHxnCdjmBtw/view?usp=drive_link). It was downloaded, unzipped, and housed in a data/ folder that was not pushed to the repository due to its size. The data in the drive was originally obtained from the following sources:

**VIIRS Data:**

The [Visible Infrared Imaging Radiometer Suite (VIIRS)](https://ladsweb.modaps.eosdis.nasa.gov/) data is remotely-sensed night lights data acquired from the Suomi satellite. It includes 4 files: two tiles (h08v05 and h08v06) per date (2021-02-07 and 2021-02-16). Those dates were chosen due to the least cloud cover, allowing for the best contrast in night lights during the power crisis.

**Roads and Houses Data:**

[Geofabrik's download site](https://download.geofabrik.de/) is a third-party distributor for [OpenStreetMap (OSM)](https://planet.openstreetmap.org/) data. Here, we can find roads and houses data for Texas (downloaded as .gpkg files).

**Socioeconomic Data:**

The [U.S. Census Bureau's American Community Survey](https://www.census.gov/programs-surveys/acs) data is census-tract level data from 2019 (downloaded as a .gbd file). 

## References

GeoFabrik. (2024). Shapefiles [Roads, Houses]. Retrieved from [https://download.geofabrik.de/](https://download.geofabrik.de/)

NASA LAADS DAAC. (2021). VIIRS [Night Light]. NASA EOSDIS Land, Atmosphere Near Real-Time Distributed Active Archive Center. Retrieved from [https://viirsland.gsfc.nasa.gov/Val_overview.html](https://viirsland.gsfc.nasa.gov/Val_overview.html)

U.S. Census Bureau. (2024). American Community Survey. U.S. Department of Commerce. Retrieved from [https://www.census.gov/programs-surveys/acs](https://www.census.gov/programs-surveys/acs)

## Acknowledgements
This analysis was adopted from [EDS223: Geospatial Analysis & Remote Sensing Homework #3](https://eds-223-geospatial.github.io/). Thank you to Ruth Oliver [@ryoliver](https://github.com/ryoliver) for preparing the data hosted on Google Drive.
