# Workflow Analysis for Anomaly detection tool (crops dataset)

## Description
This workflow is a crop anomaly detection tool that takes an image URL as input. It generates an embedding for the image, compares it to a dataset of known crop images stored in Qdrant, and determines if the image represents an unknown (anomalous) crop or a known crop based on similarity scores against predefined thresholds.

## Input Details
The workflow is triggered by an execution and receives an image URL as input.

## Process Summary
First, the workflow sets up variables for Qdrant queries. It then queries Qdrant to determine the total number of distinct crop classes. Next, it uses the Voyage.ai Embeddings API to generate an embedding vector for the input image URL. This embedding is then used to query the Qdrant collection to find the similarity of the input image with the stored cluster centers (medoids) of known crop types. Finally, a Python code node compares these similarity scores against predefined thresholds to identify if the image is an anomaly or a known crop.

## Output Details
The workflow outputs a text message indicating whether the input image is an "ALERT, we might have a new undefined crop!" or "Looks similar to [crop_name]".

## Tags
automation, n8n, production-ready, excellent, optimized, anomaly detection, crops, image analysis, Qdrant, Voyage.ai
