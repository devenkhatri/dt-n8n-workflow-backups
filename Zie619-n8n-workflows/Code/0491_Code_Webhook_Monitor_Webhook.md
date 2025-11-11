# Workflow Analysis for Dynamically Replace Images in Google Slides

## Description
This workflow allows users to automatically replace images in a Google Slides presentation by sending a POST request with the presentation ID, a unique image key, and the URL of the new image. It’s ideal for automating updates like client logos or background images across multiple slides.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint with a JSON body containing 'presentation_id', 'image_key', and 'image_url'.

## Process Summary
The workflow first validates that all required fields are present in the incoming request. If any are missing, it returns a 500 error. If valid, it fetches all slide elements from the specified Google Slides presentation using the Google Slides API. It then searches for images tagged with the provided 'image_key' in their alt text and extracts their object IDs. Finally, it sends a batch request to replace those images with the new image URL and updates the alt text to retain the key.

## Output Details
On success, the workflow returns a JSON response confirming the image was replaced; on failure (e.g., missing fields), it returns an error message via the webhook response.

## Tags
Google Slides, image replacement, automation, webhook, API integration, presentation automation, n8n
