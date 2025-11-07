# Workflow Analysis for Crop Anomaly Detection Tool

## Description
This workflow is designed to detect anomalous crop images. It takes an image URL as input, generates an embedding for the image, and then compares it against a pre-trained dataset of known crop types stored in a Qdrant vector database. If the image falls below similarity thresholds for all known crop classes, it is flagged as an anomaly.

## Input Details
The workflow is triggered by an external execution command, receiving an image URL as input.

## Process Summary
First, the workflow extracts the image URL from the trigger. It then configures Qdrant database variables and queries Qdrant to determine the number of distinct crop classes. Next, it uses the Voyage AI API to convert the input image into an embedding vector. This vector is then used to query the Qdrant database to find similarities with stored medoids (cluster centers) of known crop types. Finally, a custom Python code node compares these similarity scores against predefined thresholds for each crop type to identify if the image is an anomaly or a known crop.

## Output Details
The workflow outputs a text message indicating whether the input image is an anomaly or identifies the most similar known crop.
