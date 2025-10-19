# Workflow Analysis for Social Media Image Creator with Unsplash & Cloudinary

## Description
This workflow automates the creation of social media images by first fetching a stock photograph from Unsplash based on a search query. It then downloads the image, uploads it to Cloudinary, and applies an initial transformation. Finally, it uses a Function node to construct a modified Cloudinary URL with an additional dynamic text overlay transformation for the final image output.

## Input Details
The workflow is started manually by a user initiating the "Manual Trigger" node.

## Process Summary
The workflow is manually triggered and begins by searching Unsplash for a "coding" related landscape photo. It downloads this photo via an HTTP request and then uploads the binary file to Cloudinary. The image is transformed in Cloudinary (Cloudinary1 node) with an initial set of parameters (crop/text overlay). Finally, a Function node takes the resulting Cloudinary URL and dynamically injects a further text overlay transformation to generate the final public image URL.

## Output Details
The workflow outputs a JSON object containing the `imageUrl`, which is the public URL of the final transformed image hosted on Cloudinary with two layers of text overlays.
