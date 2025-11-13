# Workflow Analysis for [3/3] Anomaly detection tool (crops dataset)

## Description
This n8n workflow serves as an anomaly detection tool for crop images. It takes an image URL, generates embedding vectors, and compares them against predefined threshold scores of known crop types stored in a Qdrant collection. The workflow determines if the image depicts an anomaly relative to the existing crop dataset.

## Input Details
The workflow is manually triggered and receives an image URL as input, which is then used for anomaly detection.

## Process Summary
First, the workflow sets up variables for interacting with the Qdrant database. It then queries Qdrant to determine the total number of distinct crop types in the collection. Next, it sends the input image to the Voyage.ai Embeddings API to generate a vector representation. This embedding is used to search the Qdrant collection for similar crop medoids and their respective threshold scores. Finally, a Python code node compares the similarity scores against these thresholds to classify the image as either a known crop or an anomaly.

## Output Details
The workflow outputs a text message indicating whether the input image is identified as an anomaly or is similar to one of the known crop types.

## Tags
automation,n8n,production-ready,excellent,optimized
