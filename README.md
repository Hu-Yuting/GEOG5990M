# GEOG5990M Final Project
# The relationship between no-car households and public transportation usage in Leeds
# Project overview
The project aims to identify the spatial distribution of no-car households in Leeds, and the relationship between no-car households and public transportation usage across Leeds Middle Layer Super Output Areas (MSOA). The analysis joins the open Census attribute data with the spatial boundary data to produce a spatial and a non-spatial visualisation map.

Households with no cars or vans usually rely more on public transportation. Identifying the spatial distribution of no-car households and analyzing the relationship can help understand the differences in transportation demands among different areas within the city. It can also provide a more detailed reference for allocating transportation resource and planning public service, which is of significant public good. 

# Data sources
Nomis Census data (https://www.nomisweb.co.uk):
   - Leeds_MSOA_no_car_households (https://www.nomisweb.co.uk/datasets/c2021ts045)

     providing the number and percentage of households with no cars or vans
   - Leeds_MSOA_bus_use (https://www.nomisweb.co.uk/datasets/c2021ts061)
   
     providing the number and percentage of people commuting using "bus, minibus or coach"

ONS Geoportal:
   - 2021 MSOA boundary data (stored in Google Drive)

# Main variables
The project focuses on two variables:
   - No-car households percentage: the percentage of households with no cars or vans in each Leeds MSOA
   - Bus use percentage: the percentage of people using bus, minibus or coach for commuting in each Leeds MSOA

# Required packages
  - pandas
  - geopandas
  - matplotlib
  - seaborn

# Main steps
  1. Read in the two attribute datasets (Leeds_MSOA_no_car_households and Leeds_MSOA_bus_use)
  2. Explore and clean the data by removing empty rows, renaming columns, and retaining useful variables
  3. Use visualisation to check the distributions of the variables
  4. Merge the two attribute data using the common MSOA code
  5. Read in the MSOA boundary file
  6. Subset the boundary data to Leeds MSOAs
  7. Join the attribute data to the boundary data
  8. Visualisations
  9. Interpret the spatial pattern and the relationship

# The final outputs:
  - A choropleth map: showing the distribution of households with no cars or vans in Leeds MSOAs
  - A scatterplot: showing the relationship between public transportation usage and no-car households in Leeds MSOAs

# How to run the notebook
  1. Open the notebook in Google Colab
  2. Make sure the required files are available in the repository, and the large boundary file is accessible in Google Drive 
  3. Run the notebook from top to bottom
