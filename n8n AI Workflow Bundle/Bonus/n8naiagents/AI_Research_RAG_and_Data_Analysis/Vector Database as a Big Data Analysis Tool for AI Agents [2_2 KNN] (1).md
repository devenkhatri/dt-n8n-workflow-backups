# Workflow Analysis for KNN Classifier (Lands Dataset)

## Description
This n8n workflow is a K-Nearest Neighbors (KNN) classifier tool that takes an image URL as input and classifies the image into one of the predefined land types by querying a Qdrant collection of land-use images. It includes a mechanism to resolve ties in classification by increasing the number of neighbors considered.

## Input Details
The workflow is triggered by an external call, receiving an image URL via a query parameter.

## Process Summary
First, the input image URL is used to generate a vector embedding via the Voyage AI Multimodal Embeddings API. This embedding is then used to query a Qdrant database to find the K-nearest neighbor images and their associated land-use classes. A majority vote is performed on these classes to determine the most likely classification. If there is a tie in the majority vote and the neighbor limit has not been reached, the workflow iteratively increases the number of neighbors and re-queries Qdrant to resolve the tie.

## Output Details
The workflow outputs the predicted land-use class for the input image.
