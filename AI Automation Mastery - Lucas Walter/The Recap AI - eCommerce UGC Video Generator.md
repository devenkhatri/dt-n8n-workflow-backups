# Workflow Analysis for The Recap AI - eCommerce UGC Video Generator

## Description
This workflow automatically creates authentic-looking user-generated content (UGC) marketing videos for eCommerce products using AI. It starts by analyzing a product image to build a realistic influencer persona, then generates multiple natural-sounding 12-second video scripts, and finally produces the actual videos using AI video generation—delivering ready-to-use social media ads.

## Input Details
The workflow is triggered by a form submission containing a product image file and the product name.

## Process Summary
First, the product image is converted to base64 and analyzed by OpenAI's GPT-4 Vision to create a detailed profile of the ideal influencer persona. Then, Google Gemini 2.5 Pro uses this persona and the product image to generate three distinct UGC-style video scripts with frame-by-frame direction. Each script is processed individually: Gemini generates a custom first-frame image adapted to a 9:16 aspect ratio, which is then resized. This image and the corresponding script are sent to OpenAI's Sora 2 API to generate a 12-second video. The workflow polls the video status every 15 seconds until complete, then downloads and uploads the final video to a specified Google Drive folder.

## Output Details
The workflow produces multiple 12-second UGC-style marketing videos (one per script), which are automatically uploaded to a designated Google Drive folder with sequential naming.
