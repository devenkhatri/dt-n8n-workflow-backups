# Workflow Analysis for Crop Anomaly Detection Tool

## Description
This n8n workflow serves as an anomaly detection tool for crop images. It takes an image URL as input, generates an embedding, and then compares it against a pre-trained dataset of known crop types stored in Qdrant to determine if the image depicts an unknown or anomalous crop.

## Input Details
The workflow is triggered manually or via an API call, receiving an image URL as input.

## Process Summary
First, the workflow initializes Qdrant connection variables and retrieves the total count of distinct crop classes from the Qdrant collection. Then, it uses the VoyageAI Embeddings API to generate a vector embedding for the input image URL. Next, it queries the Qdrant database to find the similarity of the embedded image to the stored medoids (cluster centers) of known crop types. Finally, a Python code node compares the similarity scores against predefined thresholds to identify if the image is an anomaly or belongs to an existing crop class.

## Output Details
The workflow outputs a text message indicating whether the input image is an anomaly (a new undefined crop) or if it looks similar to a known crop type from the dataset.
