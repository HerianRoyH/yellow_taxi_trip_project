# yellow_taxi_trip_project
A simple end-to-end data engineering project that utilizes BigQuery, Python, and Looker Studio

# Project Overview
This project consists of two Google Colab notebooks: "extraction and ingestion" and "model_transformer".

The "extraction and ingestion" notebook focuses on extracting one month of yellow taxi trip data from the New York City Taxi and Limousine Commission (TLC) website, performing simple data transformation to filter out records for February 2024 where the passenger count is greater than 0, and ingesting the cleaned data into Google BigQuery. The ingested data is stored in the `yellow-taxi-trip-project` project, specifically in the `all_raw` dataset with the table named `yellow_taxi_raw`.

The "model_transformer" notebook is responsible for further data transformation, modeling, and generating final datasets or models for downstream analysis or reporting.

# Setup Instructions
To set up the environment and run the code in Google Colab notebooks, follow these steps:

1. Open the "extraction and ingestion" notebook in Google Colab.
2. Execute the code cells in the notebook sequentially. Ensure you have the necessary libraries installed and authentication set up to access Google BigQuery.
3. Similarly, open the "model_transformer" notebook in Google Colab and execute the code cells sequentially.
4. To access the project in BigQuery you may use the following credentials:
   Go to: https://console.cloud.google.com/bigquery?project=yellow-taxi-trip-project
   email_address: hrch.projects@gmail.com 
   password: Temppass0908
5. To access the line chart in Looker Studio please use this link: https://lookerstudio.google.com/reporting/1873283f-6eb1-4451-9a48-a37939ee1a0b   

# Execution Instructions
For the "extraction and ingestion" notebook:
https://colab.research.google.com/drive/1QqvkDPBg3mgnbLM8M-_bNXnT6wNllbWz?usp=sharing

1. Run the code cells to extract, transform, and ingest the data into Google BigQuery.
2. Upon completion, verify the ingested data in the BigQuery console.

For the "model_transformer" notebook:
https://colab.research.google.com/drive/1XitKj1SzgqASOyk7dFzO2GPqnp6qd_7a?usp=sharing

1. Run the code cells to perform further data transformation, modeling, and generation of final datasets or models.
2. Utilize the output for downstream analysis or reporting.

# Discussion
The project leverages Google Colab notebooks for data extraction, transformation, and ingestion into Google BigQuery. Challenges encountered during development include handling authentication with Google Cloud Platform, parsing HTML content from the NYC TLC website, ensuring data quality and consistency, and sharing of BigQuery project with unknown viewers or users.

Assumptions made during development include the availability of consistent and reliable data from the NYC TLC website and the compatibility of extracted data with BigQuery schema requirements.
