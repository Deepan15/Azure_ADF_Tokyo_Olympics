## Tokyo Olympics Data Analysis: Microsoft Azure End-to-End Pipeline Project

This repository provides a comprehensive guide on how to build and implement an end-to-end data engineering pipeline for the analysis of Tokyo Olympics data. This project takes advantage of several Microsoft Azure services, including Azure Data Lake Gen2, Azure Data Factory (ADF), Azure Synapse Analytics, Databricks, and Power BI.

## Project Overview
The goal of this project is to develop an end-to-end data pipeline to ingest, transform, analyze, and visualize historic data from the Tokyo Olympics. Initially, data is ingested into an Azure Data Lake Gen2 storage account using Azure Data Factory pipelines. Following ingestion, the data is processed and curated using Databricks Notebooks. Azure Synapse Analytics is then deployed to create a SQL database from the curated data, which is subsequently integrated into PowerBI for sophisticated analytics and visualizations.

## Project Architecture
The architecture of this data pipeline consists of the following Azure services:

* Azure Databricks for data transformation.
* Azure Data Factory for data ingestion.
* Azure Storage (Data Lake Gen2) for data storage.
* Azure Synapse Analytics for creating a SQL database.
* Power BI for data visualization

## Project Process
* Built a pipeline to extract tokyo olympics data from source a github server/webpage and load it into ADLS.
* Used copy data activity from ADF to extract data from HTTP server(github) and load it into a raw zone in ADLS.
* Used Azure Databricks to perform transformations and load it into transformed zone in ADLS.
* Created a lake database on synapse analytics pointiong out the ADLS transformed zone, so BI can serve/fetch the data from synapse analytics.
* Used PowerBi to create a dashboard based on the data from ADLS Transformed zone.


