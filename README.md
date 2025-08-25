ADF Transformation Project

## Project Overview

This project demonstrates how to use Azure Data Factory (ADF) Mapping Data Flows to transform transactional data into a single aggregated view per user and export the results to a CSV file.

Input: Transactional dataset (user_id, product_name, sales).

Transformation: Group products purchased by each user into a single row.

Output: CSV file stored in Azure Blob Storage or Data Lake.

## Architecture Workflow

<img width="1025" height="200" alt="image" src="https://github.com/user-attachments/assets/1a0ad32e-4e55-451e-8d2e-ae5dbfeb9d8d" />

source: chatGPT

Source Dataset – Load raw data (CSV, SQL, etc.) into ADF.

Aggregate Transformation – Group by user_id and collect products purchased.

Derived Column – Convert product array into a delimited string.

Sink Dataset – Write the transformed data to a CSV in Blob Storage/Data Lake.

Pipeline & Trigger – Orchestrate execution with pipelines and schedule automation.
