# Workflow Analysis for CSV to JSON Converter API

## Description
This workflow converts CSV data into JSON format. It accepts CSV input either as a file upload, raw text in the request body, or JSON-formatted CSV data, and returns the parsed JSON. It includes robust error handling and sends error notifications to a Slack channel when failures occur.

## Input Details
The workflow is triggered by a POST webhook that accepts CSV data either as a binary file, raw text/plain content, or JSON input containing CSV.

## Process Summary
The workflow begins by receiving a POST request via a webhook. A switch node routes the input based on whether it's a binary file, raw text (content-type text/plain), or JSON. Binary files are parsed using an extract-from-file node, while raw text is processed by a code node that splits the CSV by commas or semicolons and converts it into JSON objects. A conditional 'If' node checks for errors during conversion. Successful results are aggregated into a single JSON field and returned with a 200 status. Errors trigger a 500 response with an error message and also send an alert to a Slack channel.

## Output Details
The workflow returns a JSON response with either the converted data (on success) or an error message (on failure), and optionally sends error details to a Slack channel.

## Tags
CSV to JSON, data conversion, webhook API, error handling, Slack alert, n8n workflow, file processing, raw text parsing
