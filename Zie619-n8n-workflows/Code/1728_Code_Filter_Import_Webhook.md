# Workflow Analysis for [1/3 - anomaly detection] [1/2 - KNN classification] Batch upload dataset to Qdrant (crops dataset)

## Description
This workflow prepares a crop image dataset for machine learning tasks by uploading it to a Qdrant vector database. It first checks if a Qdrant collection exists, creates one if needed, indexes metadata for efficient querying, then fetches crop images from Google Cloud Storage, excludes tomato images (to later test anomaly detection), generates multimodal embeddings using the Voyage AI API in batches, and finally uploads the embeddings along with image metadata to Qdrant in batched format.

## Input Details
The workflow is triggered manually and receives no external input data, relying instead on configuration variables and files stored in a Google Cloud Storage bucket.

## Process Summary
The workflow begins by checking if a Qdrant collection named 'agricultural-crops' exists; if not, it creates one with a vector configuration for Voyage embeddings and sets up a payload index on the 'crop_name' field. It then retrieves all image objects from a Google Cloud Storage bucket with a 'agricultural-crops' prefix, constructs public URLs, and extracts crop names from file paths. Tomato images are filtered out to enable anomaly testing later. The remaining images are split into configurable batches, each assigned unique UUIDs. For each batch, the workflow sends image URLs to the Voyage AI API to generate embeddings, then uploads the embeddings, UUIDs, and metadata (crop name and image path) to Qdrant in a single batch request.

## Output Details
The workflow populates a Qdrant vector database collection with image embeddings and associated metadata (crop name and public image URL) for all non-tomato agricultural crop images from the Google Cloud Storage bucket.

## Tags
Qdrant, embedding, vector database, image processing, batch processing, Google Cloud Storage, Voyage AI, anomaly detection, KNN classification, agricultural dataset, n8n, workflow automation
