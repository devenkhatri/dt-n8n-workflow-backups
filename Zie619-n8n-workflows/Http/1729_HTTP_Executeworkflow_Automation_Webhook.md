# Workflow Analysis for [2/2] KNN classifier (lands dataset)

## Description
This workflow is a K-Nearest Neighbors (KNN) classifier designed to categorize satellite imagery of land types. It takes an image URL as input, extracts its embedding using Voyage.ai Multimodal Embeddings API, and then queries a Qdrant database to find similar pre-labeled images. The workflow uses a majority voting system to determine the image's class, and includes a loop to resolve ties by expanding the search for nearest neighbors.

## Input Details
The workflow is triggered by an external call, likely from another workflow, and receives an image URL as input.

## Process Summary
The workflow first receives an image URL and generates a multimodal embedding for it using the Voyage.ai API. It then queries a Qdrant vector database with this embedding to retrieve a set of nearest neighbor images and their associated land type labels. A majority vote is conducted on these labels to determine the most probable land type. In case of a tie in the majority vote, the workflow iteratively increases the number of neighbors queried from Qdrant by 5, up to a maximum of 100 neighbors, and repeats the majority voting process until a clear classification is achieved or the maximum limit is reached.

## Output Details
The workflow outputs the classified land type of the input image as a string, which is then returned to the calling workflow.

## Tags
automation, n8n, production-ready, excellent, optimized, KNN, classification, image, AI, machine learning, Qdrant, VoyageAI, land use, satellite imagery
