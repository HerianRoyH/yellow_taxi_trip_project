# yellow_taxi_trip_project
A simple end to end data engineering project that utilizes BigQuery, Python and Looker Studio

# Project Overview
This project consists of two Google Colab notebooks: "extraction and ingestion" and "model_transformer".

The "extraction and ingestion" notebook focuses on extracting one month of yellow taxi trip data from the New York City Taxi and Limousine Commission (TLC) website, performing simple data transformation to filter out records for February 2024 where passenger count is greater than 0, and ingesting the cleaned data into Google BigQuery. The ingested data is stored in the `yellow-taxi-trip-project` project, specifically in the `all_raw` dataset with the table named `yellow_taxi_raw`.

The "model_transformer" notebook is responsible for further data transformation, modeling, and generating final datasets or models for downstream analysis or reporting.

# Setup Instructions
To set up the environment and run the code in Google Colab notebooks, follow these steps:

1. Open the "extraction and ingestion" notebook in Google Colab.
2. Execute the code cells in the notebook sequentially. Ensure you have the necessary libraries installed and authentication set up to access Google BigQuery.
3. Similarly, open the "model_transformer" notebook in Google Colab and execute the code cells sequentially.

# Execution Instructions
For the "extraction and ingestion" notebook:

1. Run the code cells to extract, transform, and ingest the data into Google BigQuery.
2. Upon completion, verify the ingested data in the BigQuery console.

For the "model_transformer" notebook:

1. Run the code cells to perform further data transformation, modeling, and generation of final datasets or models.
2. Utilize the output for downstream analysis or reporting.

# Discussion
The project leverages Google Colab notebooks for data extraction, transformation, and ingestion into Google BigQuery. Challenges encountered during development include handling authentication with Google Cloud Platform, parsing HTML content from the NYC TLC website, and ensuring data quality and consistency.

Assumptions made during development include the availability of consistent and reliable data from the NYC TLC website and compatibility of extracted data with BigQuery schema requirements.
