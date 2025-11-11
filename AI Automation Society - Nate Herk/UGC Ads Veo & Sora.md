# Workflow Analysis for UGC Ads Veo & Sora

## Description
This workflow automatically generates AI-powered user-generated content (UGC) style videos for marketing, using either Veo 3.1 or Sora 2 models based on the configuration in a Google Sheet. It creates realistic selfie-style videos featuring a human influencer holding a product, following detailed prompts and using product photos provided in the sheet.

## Input Details
The workflow is triggered on a schedule and pulls rows marked as 'Ready' from a connected Google Sheet containing product details, ideal customer profiles, video settings, and the target AI video model.

## Process Summary
The workflow starts by fetching a 'Ready' row from a Google Sheet. It then routes the data based on the specified AI model (Veo 3.1, Nano + Veo 3.1, or Sora 2). For Veo-only jobs, it generates a video directly. For Nano + Veo jobs, it first creates an enhanced image using NanoBanana, analyzes that image with OpenAI Vision, and then generates a Veo video using that description. For Sora jobs, it creates a Sora-specific prompt and generates a video. After generation, the workflow polls for completion and updates the Google Sheet with the video URL and a 'Finished' status.

## Output Details
The workflow produces a finished UGC-style video URL and updates the original Google Sheet row with this URL and a 'Finished' status.

## Tags
AI video generation, UGC ads, Veo, Sora, Google Sheets, scheduled automation, influencer marketing, product promotion
