# GACities_Census_Maps

## Overview
This script processes Census ACS5 Summary table S1701 data to visualize poverty statistics for Georgia cities, counties, and regions. The script calculates percentages for various poverty categories, outputs the results to CSV files, and updates the census maps for GA City Solutions in ArcGIS.

## Key Features
- % Children in Poverty (S1701_C03_002E)
- % Individuals in Poverty (All Ages) (S1701_C03_001E)
- % Seniors in Poverty (>65 yrs) (S1701_C03_003E) 
<p> The script aggregates data for GMA districts based on county-level data and region numbers provided by ArcGIS. It also handles data import, processing, and output to CSV files. </p>p>

## Prerequisites
- Python 3.x
- ArcGIS Pro's Python Command Prompt (for running the script)

## Required Python Packages
- us
- census
- requests
- python-dotenv
- pandas
- arcgis

## Setup
### API and Credential Management

Ensure you have the following credentials set up in your .env file:

<code>
CENSUS_API=your_census_api_key
GAC_USERNAME=your_gac_arcgis_username
GAC_PASSWORD=your_arcgis_password
</code>


This file should be located in the same directory as the script. 


## Script Functionality

- Fetches Census Data: Uses the Census API to get poverty data for counties and cities.
- Processes Data: Aggregates county-level data to compute regional statistics.
- ArcGIS Integration: Connects to ArcGIS to retrieve and process region data.
- Generates CSV Files: Outputs processed data to CSV files stored in the GACities ArcGIS group for census maps.
- Updates Feature Layers



