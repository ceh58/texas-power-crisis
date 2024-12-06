# Texas Power Crisis
By [Carmen Hoyt](https://ceh58.github.io/) [@ceh58](https://github.com/ceh58)

This repository investigates power outages in Houston, TX resulting from the winter storm in February 2021.

**INSERT IMAGE?**

## About
In February of 2021, Texas experienced a series of extreme winter storms[^1] that exposed vulnerabilities in the power grid[^2]. The resulting power outages disproportionately affected different socioeconomic groups in Houston, Texas. Using 4 different datasets (VIIRS, roads, houses, and socioeconomic data), this analysis investigates the impacts of these power outages on the residents of the Houston metropolitan area.

[^1]: Read more about the 2021 winter storm [here](https://en.wikipedia.org/wiki/February_13%E2%80%9317,_2021_North_American_winter_storm).

[^2]: Read more about the Texas power crisis [here](https://en.wikipedia.org/wiki/2021_Texas_power_crisis).

## Skills
This analysis harnesses a few valuable skills:

- Reclassifing rasters
- Masking rasters
- Vectorizing rasters
- Transforming spatial data
- Buffering
- Mapping with tmap

I used the stars and terra packages for working with raster data and the sf package for working with vector data. 

## Repository Structure
```
├── .gitignore
├── README.md
├── texas_power_crisis.Rproj
├── texas_power_crisis.html # Rendered document
└── texas_power_crisis.qmd # Details the analysis
```
## Data Access

All the data used in this analysis was downloaded from a pre-prepared [Google Drive](https://drive.google.com/file/d/1bTk62xwOzBqWmmT791SbYbHxnCdjmBtw/view?usp=drive_link). It was downloaded, unzipped, and housed in a data/ folder that was not pushed to the repository due to its size. The data in the drive was originally obtained from the following sources:

VIIRS Data:

The [Visible Infrared Imaging Radiometer Suite (VIIRS)](https://ladsweb.modaps.eosdis.nasa.gov/)[^3] data is remotely-sensed night lights data acquired from the Suomi satellite. It includes 4 files: two tiles (h08v05 and h08v06) per date (2021-02-07 and 2021-02-16). Those dates were chosen due to the least cloud cover, allowing for the best contrast in night lights during the power crisis.

[^3]: Read more about VIIRS [here](https://en.wikipedia.org/wiki/Visible_Infrared_Imaging_Radiometer_Suite).

Roads and Houses Data:

[Geofabrik's download site](https://download.geofabrik.de/) is a third-party distributor for [OpenStreetMap (OSM)](https://planet.openstreetmap.org/) data. Here, we can find roads and houses data for Texas (downloaded as .gpkg files).

Socioeconomic Data:

The [U.S. Census Bureau's American Community Survey](https://www.census.gov/programs-surveys/acs) data is census-tract level data from 2019 (downloaded as a .gbd file). 

## References



## Acknowledgements
This analysis was adopted from [EDS223: Geospatial Analysis & Remote Sensing](https://eds-223-geospatial.github.io/). Thank you to [Ruth Oliver]() for preparing the VIIRS data.


