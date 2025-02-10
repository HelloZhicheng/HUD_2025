# **US Census Bureau Data Retrieval**

## **Overview**
This folder retrieves and processes **social**, **economic**, and **health** data from the US Census Bureau API for census tracts in Michigan (state code 26) and Ohio (state code 39). The data spans the years 2010 to 2020.

## **Features**
1. Downloads Census Bureau data for Michigan and Ohio at the census tract level.
2. Handles differences in census tract boundaries for the 2020 dataset compared to the 2010–2019 period.
3. Combines retrieved data with a census tract summary file.
4. Processes and saves data as year-specific CSV files.

## **Required Libraries**
Install the following R libraries before running the script:
install.packages(c("requests", "pandas"))

## **Input Data**
1. **Census Bureau API**: Data retrieved using API calls with specific variable codes.
2. **Census Tract Summary File**: A file named censustract_summary.xlsx containing census tract information for (1) 2010–2019: Data stored in the 2010_2019 sheet; (2) 2020: Data stored in the 2020 sheet. Ensure this file is in the same directory as the script.

## **Outputs**
Yearly combined datasets from 2010 to 2020. Each file contains merged data from the Census Bureau API and the census tract summary.

## **Usage**
1. Place the script and **censustract_summary.xlsx** in the same directory.
2. Run the script in R or RStudio.

## **Customization**
1. **API Variables**: Adjust variables in the `url_part1` and `url_part2` strings to include additional or alternative census variables.
2. **Years**: Update the `years` list to fetch data for different time periods.