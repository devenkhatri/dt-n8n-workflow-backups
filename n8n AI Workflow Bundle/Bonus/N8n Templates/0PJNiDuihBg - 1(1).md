# Workflow Analysis for AI Facebook Ad Spy Tool

## Description
This workflow automates the process of spying on Facebook ads by scraping the Facebook Ad Library, filtering ads based on engagement, and using AI to analyze and rewrite ad copy. It helps advertising agencies gain strategic intelligence on competitor ads.

## Input Details
This workflow is manually triggered and initiates by scraping Facebook Ad Library data for ads related to "ai automation" from an external API.

## Process Summary
The workflow first fetches Facebook ad data from an Apify scraper, then filters these ads to include only those with over 1000 likes. It categorizes the filtered ads into video, image, or text types. Video ads are downloaded, uploaded to Google Drive, then sent to Gemini for detailed description, followed by OpenAI for summarization and ad copy rewriting. Image ads are directly analyzed and summarized by OpenAI. Text-only ads are summarized and rewritten by OpenAI. Each type of ad is processed in batches.

## Output Details
The workflow outputs detailed analysis, including original ad information, AI-generated summaries, rewritten ad copy, and image/video prompts, by appending them as new rows to a Google Sheet named "Facebook Ad Library Analyzer DB".
