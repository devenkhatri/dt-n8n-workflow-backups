# Workflow Analysis for AI Facebook Ad Spy Tool

## Description
This workflow acts as an AI-powered Facebook ad spy tool. It automatically scrapes recent "AI automation" advertisements from the Facebook Ad Library, filters them by popularity (over 1000 likes), and then uses advanced AI models (Gemini and OpenAI) to analyze the ad content, including videos and images, before generating comprehensive summaries and rewritten ad copy for strategic marketing intelligence, all stored in a Google Sheet.

## Input Details
The workflow is manually triggered and initiates an API call to an ad scraping service to retrieve Facebook Ad Library data for "AI automation" ads.

## Process Summary
1. The workflow is manually initiated to scrape Facebook Ad Library for "AI automation" ads from the last 7 days.
2. It filters these ads to include only those with over 1000 likes.
3. Ads are then categorized into video, image, or text types for separate processing.
4. Video ads are downloaded, uploaded to Google Drive, then transferred to Google Gemini for detailed analysis, and finally summarized and rewritten using OpenAI.
5. Image ads are analyzed using OpenAI, which also summarizes the ad and rewrites its copy. Text-only ads are directly summarized and rewritten by OpenAI.
6. All processed ad data, including summaries and rewritten copy, is then appended to a Google Sheet.

## Output Details
The workflow produces detailed analyses, summaries, and rewritten ad copy for each processed Facebook ad, storing this information in a Google Sheet.
