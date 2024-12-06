# Investigating redlined neighborhoods in LA County

![Image](https://s3.amazonaws.com/holc/tiles/CA/LosAngeles1/1939/holc-scan.jpg)

Image Credit:Mapping Inequalityhttps://dsl.richmond.edu/panorama/redlining/data/CA-LosAngeles
### Purpose
This repository aims to investigate the imbalance of bird observations in historically redlined neighborhoods in LA county. In the 1930's the Home Owners' Loan Corporation (HOLC) rated neighborhood blocks on their perceived safety. The ranking system A (green), B (blue), C (yellow), and D (red) was used to stop access for loans in neighborhoods of lower ratings, known as redlining. This practice has negatively impacted not only the community economy, but also its health. Redlined neighborhoods are considerably hotter due to having less local greenery. 

The HOLC's rating system has had a ripple effect on these communities over the decades since it started. Recently, studies have shown that redlined neighborhoods have fewer biodiversity observations. Citizen science is becoming more influential in modern day data collection, however, Ellis-Soto et al. (2023) discovered that redlined neighborhoods are the most undersampled areas across 195 cities. As policy is implemented from this data, it is important to understand the gap from this sampling bias. 

### Highlights of Analysis
- Load in geospatial data using `sf`
- `Filter` data to LA County
- Create map of redlined neighborhoods
- `Join` spatial data for comparitive analysis
- `Summarize` low income, particulate matter, and low life expectancy by HOLC grade
- Use `st_intersects` for bird observations across HOLC grades
   
### Dataset Descriptions
#### EJ Screen Data
The United States Environmental Protection Agency's EJScreen: Environmental Justice Screening and Mapping Tool data will be used to provide data for the US Census tract and block group levels. This data can be downloaded directly from the [EPA Website](https://www.epa.gov/ejscreen/download-ejscreen-data). Limitations of this dataset can also be found on [EPA's site](https://www.epa.gov/ejscreen/limitations-and-caveats-using-ejscreen).

#### HOLC Redlining
Home Owner's Loan Corporation data can be found [here](https://dsl.richmond.edu/panorama/redlining/data). This data is from the [Digital Scholarship Lab](https://dsl.richmond.edu/) at the University of Richmond and is a part of their [Mapping Inequality](https://dsl.richmond.edu/panorama/redlining/#loc=5/39.1/-94.58). 

#### Biodiversity Observations
Data on bird observations can be found from the [Global Biodiversity Information Facility](https://www.gbif.org/). They are the largest compiler of biodiversity observations in the world. Our data is looking at bird observations from 2021 to present. 

### Authors 
A special thanks to [Ruth Oliver](https://github.com/ryoliver) for guidance in [EDS 223](https://eds-223-geospatial.github.io/) in the completion of this work. 

### References & Acknowledgements
Ellis-Soto, D., Chapman, M., & Locke, D. H. (2023). Historical redlining is associated with increasing geographical disparities in bird biodiversity sampling in the United States. Nature Human Behaviour, 1-9.

GBIF.org (13 October 2024) [GBIF Occurence Download](https://www.gbif.org/)

Nelson, R. K., Winling, L, et al. (2023). Mapping Inequality: Redlining in New Deal
America. (Digital Scholarship Lab)[https://dsl.richmond.edu/panorama/redlining].

United States Environmental Protection Agency. 2024 version. [EJScreen](www.epa.gov/ejscreen).
Retrieved: 10/4/24 from www.epa.gov/ejscreen

