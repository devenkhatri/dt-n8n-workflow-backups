# Workflow Analysis for Upload Post Images

## Description
This workflow automates the process of fetching multiple images and posting them to social media platforms like Instagram and TikTok.

## Input Details
The workflow is triggered manually and fetches two images from a webhook URL.

## Process Summary
1. The workflow starts manually.
2. It retrieves two images from a predefined webhook URL.
3. The images' binary data are renamed to 'photo1' and 'photo2'.
4. These renamed images are then combined into a single data item.
5. Finally, the workflow sends the merged images, along with post details, to separate API endpoints for Instagram and TikTok.

## Output Details
The workflow sends HTTP POST requests containing image data and post information to an external API for both Instagram and TikTok platforms.

## Tags
automation, n8n, production-ready, excellent, optimized
