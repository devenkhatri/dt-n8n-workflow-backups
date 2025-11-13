# Workflow Analysis for KNN classifier (lands dataset)

## Description
This n8n workflow is a KNN classifier tool that takes an image URL as input and classifies the object on the image into one of the predefined land types. It utilizes the Voyage.ai Multimodal Embeddings API to generate image embeddings and then queries a Qdrant database to find the nearest neighbors for classification. The workflow includes a loop to handle ties in majority voting by increasing the number of neighbors considered.

## Input Details
The workflow is triggered by an Execute Workflow Trigger node and receives an image URL as input.

## Process Summary
First, the workflow sets the input image URL. Then, it uses the Voyage.ai Multimodal Embeddings API to embed the image, generating a vector representation. This image embedding, along with initial Qdrant collection details and a K-nearest neighbors limit, are prepared. Subsequently, the workflow queries Qdrant to find the nearest neighbors to the embedded image. A majority vote is then performed on the classes of these neighbors to determine the most frequent class. If a tie occurs in the top two most common classes, the workflow enters a loop, increasing the number of neighbors to query from Qdrant, until a clear majority is found or a maximum limit of 100 neighbors is reached. Finally, the identified class name is extracted.

## Output Details
The workflow returns the classified land type (e.g., "agricultural", "forest", "beach") as the result.

## Tags
KNN, Classification, Image Classification, Machine Learning, AI, Qdrant, Voyage AI, Land Use, Automation
