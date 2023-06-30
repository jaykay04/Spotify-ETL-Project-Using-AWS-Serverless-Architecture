# Spotify ETL Project Using AWS Serverless Architecture

## Introduction
This Project simply demonstrates how to build a robust automated and scalable data pipeline for extracting, transforming and loading Spotify data using AWS Serverless Data architecture.   

Data was extracted from Spotify API and stored in S3 bucket. The extraction process was automated using Cloudwatch Events and designed to run every 24 hours. After extraction, the data was transformed and stored back in S3 with a S3 event trigger activated to automate the cleaning process as well.   

In order to allow the analytics team consume the data in a structured format, AWS Glue was used to crawl the data from S3 and saved it in a table format inside the spotify database in AWS Glue Data Catalogue.

Finally, AWS Athena was deployed to query the data and run analytics so as to derive useful and actionable insights to aid Data Driven decisions.

## AWS Services and Development Environment
* Jupyter Notebook
* AWS Lambda
* S3
* CloudWatch
* AWS Glue
* AWS Athena

## Libraries 
```
pip install numpy as py
pip install pandas as pd
import spotipy
from spotipy.oauth2 import SpotifyClientCredentials
```
## Architecture Diagram
