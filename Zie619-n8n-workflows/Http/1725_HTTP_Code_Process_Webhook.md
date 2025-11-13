# Workflow Analysis for Convert Parquet, Avro, ORC & Feather via ParquetReader to JSON

## Description
This workflow automates the conversion of various columnar data formats such as Parquet, Avro, ORC, and Feather into JSON format by sending the uploaded file to an external API for processing and then parsing the API's response.

## Input Details
This workflow is triggered by a POST request to a webhook, which receives a file in Parquet, Avro, ORC, or Feather format as multipart form data.

## Process Summary
First, the workflow receives a file upload via a webhook. Next, it sends this received file as multipart form data to an external Parquet API for conversion. Finally, it parses the API's response, specifically converting stringified JSON data and metadata fields into structured JSON objects and arrays.

## Output Details
The workflow returns the parsed JSON data, including the converted file content and metadata, as the response to the initial webhook call.

## Tags
Data Conversion, File Processing, API Integration, Webhook, Parquet, Avro, ORC, Feather, JSON, Automation
