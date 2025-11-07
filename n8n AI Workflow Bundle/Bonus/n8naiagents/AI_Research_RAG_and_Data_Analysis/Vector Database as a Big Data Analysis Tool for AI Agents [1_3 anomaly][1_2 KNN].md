# Workflow Analysis for Batch Upload of Crop Image Dataset to Qdrant for Anomaly Detection and KNN Classification

## Description
This workflow is designed to prepare an agricultural crops image dataset for machine learning tasks like anomaly detection and K-Nearest Neighbors (KNN) classification. It fetches crop images from Google Cloud Storage, processes them, generates multimodal embeddings using Voyage AI, and then uploads these embeddings along with relevant metadata to a Qdrant vector database. The workflow also sets up the Qdrant collection and creates necessary indexes.

## Input Details
The workflow is manually triggered and retrieves agricultural crop image data from a specified Google Cloud Storage bucket.

## Process Summary
The workflow begins by setting up Qdrant cluster variables and checking for the existence of the target Qdrant collection; if it doesn't exist, a new collection is created with a 'voyage' vector and a 'crop_name' payload index. It then fetches image objects from Google Cloud Storage, extracts public links and crop names, and filters out 'tomato' images to aid in anomaly detection testing. The remaining images are batched, assigned unique IDs, and formatted for the Voyage AI API. Finally, the workflow sends these batches to Voyage AI for multimodal embedding generation and then uploads the resulting image embeddings, unique IDs, and metadata (crop name, image path) to the Qdrant collection.

## Output Details
The workflow populates a Qdrant vector database collection named "agricultural-crops" with image embeddings and associated metadata, making the data ready for vector search and machine learning applications.
