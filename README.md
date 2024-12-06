# Investigating redlined neighborhoods in LA County
This repository investigates the number of bird observations in  historically redlined neighborhoods in LA county

### Purpose
This repository aims to investigate the imbalance of bird observations in historically redlined neighborhoods in LA county. In the 1930's the Home Owners' Loan Corporation (HOLC) rated neighborhood blocks on their perceived safety. The ranking system A (green), B (blue), C (yellow), and D (red) was used to stop access for loans in neighborhoods of lower ratings, known as redlining. This practice has negatively impacted not only the community economy, but also its health. Redlined neighborhoods are considerably hotter due to having less local greenery. 

The HOLC's rating system has had a ripple effect on these communities over the decades since it started. Recently, studies have shown that redlined neighborhoods have fewer biodiversity observations. Citizen science is becoming more influential in modern day data collection, however, Ellis-Soto et al. (2023) discovered that redlined neighborhoods are the most undersampled areas across 195 cities. As policy is implemented from this data, it is important to understand the gap from this sampling bias. 

### Highlights of Analysis
- Load in geospatial data using `sf`
- Filter data to LA County
- Create map of redlined neighborhoods
- Join spatial data for comparitive analysis
- Summarize low income, particulate matter, and low life expectancy by HOLC grade
- Use `st_intersects` for bird observations across HOLC grades
   
### Dataset Descriptions

### Authors (for collaborative work)

### References & Acknowledgements
