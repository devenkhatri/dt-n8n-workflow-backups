# Workflow Analysis for [3/3] Anomaly detection tool (crops dataset)

## Description
This workflow is an anomaly detection tool for crop images. It takes an image URL as input, generates an embedding for the image, and then compares it against a predefined dataset of crop images in a Qdrant database to identify if the input image represents an unknown or anomalous crop.

## Input Details
This workflow is triggered by an execution and receives an image URL as input.

## Process Summary
First, the workflow extracts the input image URL and sets up variables for querying the Qdrant database. It then retrieves the total number of distinct crop types from the Qdrant collection. Next, it sends the input image to the Voyage AI Embeddings API to generate a vector embedding. This embedding is used to query the Qdrant database to find the similarity of the input image to known crop cluster centers (medoids). Finally, a Python script compares these similarity scores against pre-defined thresholds for each crop type to determine if the image is an anomaly or a known crop.

## Output Details
The workflow outputs a text message indicating whether the input image is an anomaly or similar to a known crop type.

## Tags
automation, n8n, production-ready, excellent, optimized, anomaly detection, crops, image analysis, AI, machine learning
