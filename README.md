# GEOG5990M Spatial data science report
## The relationship between no-car households and public transportation usage in Leeds
## Project overview
The project focuses on the spatial distribution of no-car households in Leeds, and the relationship between no-car households and public transportation usage. Using the open Census attribute data and the spatial boundary data to conduct the data search and download, data exploration, data cleaning and processing, data join and visualization at the  Middle Layer Super Output Areas (MSOA) level. And also producing a spatial and a non-spatial visualisation map to draw the conclusion.

Households with no cars or vans usually rely more on public transportation. Identifying the spatial distribution of no-car households and analyzing the relationship can help understand the differences in transportation demands among different areas within the city. It can also provide a more detailed reference for allocating transportation resource and planning public service, which is of significant public good. 

## Data sources
### Nomis Census data (https://www.nomisweb.co.uk):
#### Dataset 1: Car or van availability (https://www.nomisweb.co.uk/datasets/c2021ts045)
      - the number of households with no cars or vans
      - the percentage of households with no cars or vans

#### Dataset 2: Method used to travel to work (https://www.nomisweb.co.uk/datasets/c2021ts061)
      - the number of people commuting using "bus, minibus or coach"
      - the percentage of people commuting using "bus, minibus or coach"

### ONS Geoportal:
#### Dataset 3:  2021 MSOA boundary data (stored in Google Drive)
      - join attribute data and the spatial data
      - create a spatial distribution map of Leeds MSOA

## Data in GitHub repository
      - Leeds_MSOA_no_car_households.csv
      - Leeds_MSOA_bus_use.csv
      - leeds_msoa_boundaries.geojson

## Main variables
The project focuses on two variables:
   - No-car households percentage: the percentage of households with no cars or vans in each Leeds MSOA
   - Bus use percentage: the percentage of people using bus, minibus or coach for commuting in each Leeds MSOA

## Required packages
  - pandas
  - geopandas
  - matplotlib
  - seaborn

## Main steps
  1. Read in the two attribute datasets (Leeds_MSOA_no_car_households and Leeds_MSOA_bus_use)
  2. Explore and clean the data by removing empty rows, renaming columns, and retaining useful variables
  3. Use visualisation to check the distributions of the variables
  4. Merge the two attribute data using the common MSOA code
  5. Read in the MSOA boundary file
  6. Subset the boundary data to Leeds MSOAs
  7. Join the attribute data to the boundary data
  8. Visualisations
  9. Interpret the spatial pattern and the relationship

## The final outputs
  - A choropleth map: showing the distribution of households with no cars or vans in Leeds MSOAs
  - A scatterplot: showing the relationship between public transportation usage and no-car households in Leeds MSOAs

## The results
  1. No-car households in Leeds show an uneven distribution, with a high percentage in the central areas and a low percentage in the outer areas. 
  2. The areas with a high percentage of no-car households usually rely more on public transportation.

## How to run the notebook
  1. Open the notebook in Google Colab
  2. Make sure the required files are available in the repository, and the large boundary file is accessible in Google Drive 
  3. Run the notebook from top to bottom
