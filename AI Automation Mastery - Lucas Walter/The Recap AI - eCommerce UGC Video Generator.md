# Workflow Analysis for The Recap AI - eCommerce UGC Video Generator

## Description
This n8n workflow automates the creation of authentic User-Generated Content (UGC) style marketing videos for eCommerce products using advanced AI. By simply uploading a product image and providing its name, the workflow generates multiple realistic influencer-style video ads, complete with detailed scripts, influencer personas, and video production.

## Input Details
The workflow is triggered by a web form submission that receives a product image and the product name.

## Process Summary
First, OpenAI's vision API analyzes the uploaded product image to create a detailed profile of an ideal influencer. Next, Google Gemini 2.5 Pro uses this persona and product details to generate multiple authentic 12-second UGC video scripts, each with a frame-by-frame breakdown. For each script, Gemini 2.5 Flash then adapts the product image into a custom first frame for the video. Finally, Sora 2 API generates the actual UGC video, which is then uploaded to Google Drive upon completion, after polling for its generation status.

## Output Details
The workflow produces multiple 12-second UGC marketing videos in 720x1280 resolution, which are then uploaded to a specified Google Drive folder.
