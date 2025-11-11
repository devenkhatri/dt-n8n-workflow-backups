# Workflow Analysis for [1/3 - anomaly detection] [1/2 - KNN classification] Batch upload dataset to Qdrant (crops dataset)

## Description
This workflow uploads agricultural crop images from Google Cloud Storage to a Qdrant vector database for use in anomaly detection and KNN classification. It checks if the Qdrant collection exists, creates it if needed, indexes metadata for efficient querying, processes images in batches, generates multimodal embeddings using the Voyage AI API, and uploads the embeddings along with crop metadata to Qdrant—excluding tomato images to enable anomaly testing.

## Input Details
The workflow is triggered manually and receives no external input data, relying instead on configuration variables and images stored in a Google Cloud Storage bucket.

## Process Summary
First, the workflow checks if a Qdrant collection named 'agricultural-crops' exists; if not, it creates one with a vector configuration for Voyage embeddings and sets up a payload index on the 'crop_name' field. It then retrieves all crop images from a Google Cloud Storage bucket, constructs public URLs, and extracts crop names from the folder paths. Tomato images are filtered out to support anomaly detection testing. The remaining images are split into configurable-sized batches, and UUIDs are generated for Qdrant point IDs. Each batch is sent to the Voyage AI API to generate multimodal embeddings, and the resulting embeddings along with metadata are uploaded to Qdrant in batch format.

## Output Details
The workflow populates a Qdrant collection with vector embeddings and associated crop metadata for non-tomato agricultural images, enabling downstream anomaly detection and classification tasks.

## Tags
anomaly detection, KNN classification, Qdrant, vector database, Voyage AI, Google Cloud Storage, batch processing, image embeddings, multimodal AI, n8n workflow
