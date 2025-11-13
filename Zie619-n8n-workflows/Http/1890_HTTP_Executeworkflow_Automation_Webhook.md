# Workflow Analysis for [2/2] KNN classifier (lands dataset)

## Description
This n8n workflow classifies satellite imagery into predefined land-use types using a K-Nearest Neighbors (KNN) approach. It takes an image URL as input, generates an embedding for it, queries a Qdrant database of pre-labeled land images, and determines the most probable land class.

## Input Details
The workflow is triggered by an external call, receiving an image URL as its primary input.

## Process Summary
First, the input image URL is used to generate a multimodal embedding via the Voyage.ai API. This embedding is then used to query a Qdrant database, retrieving a specified number of nearest neighbor land images. A majority vote among the neighbors' labels determines the initial classification. If a tie occurs between the top two classes and the neighbor limit has not exceeded 100, the number of neighbors is incrementally increased, and the query and voting steps are repeated until a clear majority or the limit is reached.

## Output Details
The workflow outputs the identified land-use class as a string, which is returned to the calling system.

## Tags
automation, n8n, production-ready, excellent, optimized, KNN Classifier, Image Classification, Machine Learning, AI, Qdrant, Voyage AI, Land Use
