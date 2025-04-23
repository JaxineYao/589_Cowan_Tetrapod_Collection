# North American Mammal Distribution Analysis

## Project Overview
This project analyzes the spatial distribution patterns of mammals across North America (USA and Canada) using point pattern analysis techniques. The analysis includes kernel density estimation, point pattern modeling, and investigation of the relationship between mammal occurrences and elevation.

## Data Sources
- Mammal occurrence data from GBIF (Global Biodiversity Information Facility)
- Elevation data: WorldClim elevation dataset (10-minute resolution)
- Geographic boundaries: Natural Earth Data for North America

## Analysis Methods
The project implements several spatial analysis techniques:
1. **Data Preprocessing**
   - Cleaning and filtering occurrence data
   - Spatial projection (EPSG:3857)
   - Geographic filtering for USA and Canada

2. **Spatial Analysis**
   - Kernel density estimation to visualize occurrence hotspots
   - Point Pattern Analysis (PPA)
   - Homogeneous and inhomogeneous Poisson point process models
   - G-function analysis with Monte Carlo envelopes

3. **Environmental Analysis**
   - Integration of elevation data
   - Analysis of elevation effects on mammal distribution
   - Residual analysis for model evaluation

## Key Findings
- Created density maps showing mammal occurrence hotspots in North America
- Analyzed spatial clustering patterns using point process models
- Investigated the relationship between elevation and mammal distribution
- Generated smoothed Pearson residuals to assess model fit

## Dependencies
- R packages:
  - `readr`: Data reading
  - `sf`: Spatial data handling
  - `dplyr`: Data manipulation
  - `spatstat`: Point pattern analysis
  - `rnaturalearth`: Geographic data
  - `raster`: Raster data processing

## Project Structure

```
├── data/
│ ├── 0014155-250402121839773 # Mammal occurrence data
│ └── wc2.1_10m_elev.tif # Elevation data
├── project.Rmd # R Markdown file for analysis
├── project.html # rendered HTML output
└── README.md