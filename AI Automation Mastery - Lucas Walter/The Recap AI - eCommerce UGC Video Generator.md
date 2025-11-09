# Workflow Analysis for The Recap AI - eCommerce UGC Video Generator

## Description
This workflow automatically creates authentic-looking user-generated content (UGC) marketing videos for eCommerce products by analyzing a product image, generating a realistic influencer persona, writing natural-sounding ad scripts, and producing short 12-second videos using AI video generation.

## Input Details
The workflow is triggered by a form submission containing a product image file and a product name.

## Process Summary
First, the product image is converted to base64 and analyzed by OpenAI's GPT-4 Vision to generate a detailed profile of an ideal influencer persona for the product. Then, Google Gemini 2.5 Pro uses this persona and the product image to create three unique 12-second UGC video scripts with frame-by-frame camera directions and natural dialogue. Each script is processed individually: Gemini generates a custom first-frame image adapted to UGC aesthetics, which is resized to 720x1280. This frame and its corresponding script are sent to OpenAI's Sora 2 API to generate a video. The workflow polls the video status every 15 seconds until completion, then downloads and uploads the finished video to a specified Google Drive folder.

## Output Details
The workflow produces multiple 12-second UGC-style marketing videos (one per script) and uploads them to a designated Google Drive folder with organized naming.

## Tags
eCommerce, UGC, video generation, AI marketing, influencer persona, OpenAI, Gemini, Sora, Google Drive, product promotion
