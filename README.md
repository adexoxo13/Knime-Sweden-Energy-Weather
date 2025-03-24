# Knime-Sweden-Energy-Weather

## Energy Production and Weather Analysis in Sweden

A KNIME workflow analyzing the relationship between Sweden's energy production and weather patterns using data from SCB and SMHI APIs.

## Project Overview

This project investigates how weather conditions affect energy production in Sweden by:
1. Collecting energy production data from Statistics Sweden (SCB)
2. Gathering weather data from Swedish Meteorological Institute (SMHI)
3. Processing and joining the datasets
4. Visualizing relationships
5. Performing cluster analysis

## Workflow Components

### 1. Data Collection
- **SCB Energy Data**: Collected via SCB's API (modified from provided example)
- **SMHI Weather Data**: Collected from at least 4 stations with 3 variables:
  - Selected variables: [List your chosen variables, e.g., temperature, precipitation, wind speed]
  - Selected stations: [List your stations with motivations]

### 2. Data Processing
- Data cleaning and wrangling
- Monthly aggregation with multiple statistics (mean, median, min, max, etc.)
- Joining of weather and energy datasets

### 3. Analysis
- 3+ visualizations showing energy-weather relationships
- Hierarchical clustering to identify monthly patterns
- Cluster interpretation describing typical months in each group

## How to Use

1. Open `workflows/Energy_Weather_Analysis.knwf` in KNIME
2. Ensure you have these KNIME extensions installed:
   - KNIME REST Client nodes
   - KNIME JavaScript nodes
   - KNIME Plotly nodes (for visualizations)
3. The workflow should run without additional configuration

## Key Findings

[Write 2-3 bullet points summarizing your most interesting findings]
- Example: "Temperature showed the strongest correlation with solar energy production"
- Example: "Three distinct seasonal patterns emerged from cluster analysis"

## Visualizations

![Example Visualization](images/plot1.png)
*Caption explaining what this visualization shows*

## Acknowledgements

- Data sources:
  - [SMHI API](https://www.smhi.se/data/)
  - [SCB API](https://www.scb.se/api/)
