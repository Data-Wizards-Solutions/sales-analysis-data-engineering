# Sales Analysis ETL Application

## Overview
This application is designed to perform Extract, Transform, and Load (ETL) operations to retrieve and process a base table. The processed data will be ingested into a database of your choice (preferably a smart choice based on scalability and performance). The application also provides two key endpoints for data analysis and insights.

## Data Sources
The application includes the following data sources located in [this directory](https://novera-my.sharepoint.com/:f:/g/personal/maarten_degroodt_datawizards_io/Ev44l_rfC_JEnQRMhYb0fhsBCA1ZJRr0wEHSWBKv5Hqh4Q?e=R6cEO7):
- `city.csv`
- `customer.csv`
- `installation.csv`
- `product_category.csv`
- `product.csv`

## Objectives
1. **ETL Process**: Write an ETL pipeline to retrieve and process a base table from the provided data sources.
2. **Database Ingestion**: Ingest the processed data into a database of your choice.
3. **API Endpoints**:
   - **/lat-lon-revenue**: Given a location (latitude and longitude), calculate the revenue of last year's installations in the nearest city that is generating the highest revenue, and return this in a json including his/her id and email
   - **/city-revenue**: Return the total revenue of the last year for a specified location by city name, make sure it's robust.
4. Docker in which to serve the API endpoint

## Instructions
1. **ETL Pipeline**:
   - Extract data from the provided CSV files.
   - Transform the data to create a base table that includes relevant fields for analysis.
   - Load the transformed data into a database.

2. **Database Selection**:
   - Choose a database that supports efficient querying and scalability.

3. **API Endpoints Implementation**:
   - The `/lat-lon-revenue` endpoint:
     - Input: JSON with `latitude` and `longitude` fields
     - Output: JSON with `customer_id`, `email`, and `revenue` fields
   - The `/city-revenue` endpoint:
     - Input: JSON with `city_name` field
     - Output: JSON with `city_name` and `total_revenue` fields
   - Ensure proper error handling and validation for both endpoints.

4. **Docker in which to serve the app**



## Notes
- You should be able to finish the case in 4 hours.
- Use Python as the primary programming language.
- Follow best practices for ETL and database design.
- Ensure the endpoints are optimized for performance.
- Document your code and provide clear instructions for running the application.


