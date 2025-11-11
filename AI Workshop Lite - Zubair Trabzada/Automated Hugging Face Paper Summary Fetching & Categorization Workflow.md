# Workflow Analysis for [3/3] Anomaly detection tool (crops dataset)

## Description
This workflow detects whether a given crop image is anomalous (i.e., not part of the known crop types) by comparing it against a preprocessed dataset of agricultural crops stored in a Qdrant vector database.

## Input Details
The workflow is triggered manually or via API with an input containing an image URL representing a crop.

## Process Summary
The workflow starts by receiving an image URL. It then uses the Voyage AI multimodal embedding API to generate a vector embedding of the image. Concurrently, it retrieves metadata about the known crop classes from Qdrant to determine how many crop types exist. Using the generated embedding, it queries the Qdrant collection to find the most similar cluster medoids (representative crop images) and compares the similarity scores against precomputed thresholds. If the image’s similarity score exceeds the threshold for any known crop class, it is classified as that crop; otherwise, it is flagged as an anomaly.

## Output Details
The workflow outputs a text message indicating whether the input image matches a known crop type or represents a potential anomaly.

## Tags
anomaly-detection, crops, image-classification, qdrant, voyage-ai, vector-embedding, agricultural-data
