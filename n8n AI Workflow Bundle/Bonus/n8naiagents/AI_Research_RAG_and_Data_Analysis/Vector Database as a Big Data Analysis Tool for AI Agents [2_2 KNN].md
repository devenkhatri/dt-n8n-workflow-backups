# Workflow Analysis for KNN Classifier for Land Use Images

## Description
This n8n workflow is a KNN (K-Nearest Neighbors) classifier designed to categorize satellite imagery into various land use types. It takes an image URL as input, generates a multimodal embedding for the image using the Voyage AI API, and then queries a Qdrant vector database to find similar images with pre-labeled land-use classes. The workflow performs a majority vote among the nearest neighbors to determine the input image's class. It includes a loop to increase the number of neighbors considered if there's a tie in the initial classification, ensuring a definitive class is returned.

## Input Details
The workflow is triggered by an Execute Workflow Trigger and receives an image URL within its query parameter (e.g., {"query": {"imageURL": "..."}}).

## Process Summary
1. The workflow starts by extracting the imageURL from the input.
2. It then calls the Voyage AI Multimodal Embeddings API to generate a vector embedding for the provided image.
3. Next, it queries a Qdrant vector database, specifically the 'land-use' collection, using the generated image embedding to find the 'k' nearest neighbor images.
4. A Python code node performs a majority vote on the landscape_name payload of these neighbors to identify the most frequent class.
5. If there's a tie between the top two classes and the number of neighbors checked is less than 100, the workflow increases the limitKNN by 5 and repeats the Qdrant query and majority vote steps.
6. Once a clear majority is found or the limit of 100 neighbors is reached, the workflow proceeds.

## Output Details
The workflow outputs the identified land-use class (e.g., 'buildings', 'forest', 'river') as a string to the calling workflow.
