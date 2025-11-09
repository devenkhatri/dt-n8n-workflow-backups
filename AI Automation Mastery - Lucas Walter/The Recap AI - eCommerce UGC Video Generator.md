# Workflow Analysis for The Recap AI - eCommerce UGC Video Generator

## Description
This workflow automatically creates authentic-looking user-generated content (UGC) marketing videos for eCommerce products using AI. It starts with a product image and name, then generates an ideal influencer persona, writes multiple realistic 12-second video scripts, and finally produces and uploads the actual videos to Google Drive.

## Input Details
The workflow is triggered by a form submission containing a product image file and product name.

## Process Summary
First, the product image is analyzed by OpenAI's vision model to create a detailed profile of the ideal influencer for promoting the product. Then, Google Gemini generates multiple authentic UGC video scripts (12 seconds each) based on this persona and the product details. Each script is processed individually to generate a custom first frame that adapts the product image to UGC aesthetic, which is then used by OpenAI's Sora 2 API to generate the actual video. The workflow monitors video generation status and uploads completed videos to a specified Google Drive folder.

## Output Details
The workflow produces multiple 12-second UGC-style marketing videos in 720x1280 format that are automatically uploaded to Google Drive with organized naming.

## Tags
eCommerce, UGC, video generation, AI, marketing automation, influencer content, OpenAI, Gemini, Sora, Google Drive
