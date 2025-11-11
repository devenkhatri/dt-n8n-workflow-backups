# Workflow Analysis for Automate LinkedIn Posts with AI

## Description
This workflow automatically publishes AI-enhanced LinkedIn posts with images on a scheduled basis by pulling content from a Notion database, refining the text using OpenAI, and updating the post status once published.

## Input Details
The workflow is triggered daily at 3 PM and fetches data from a Notion database containing LinkedIn post content, including text and an image URL, for the current date.

## Process Summary
The workflow starts by querying a Notion database for entries scheduled for the current day. It retrieves all content blocks (text and image) from the Notion page linked in the entry. The text is sent to an OpenAI assistant to be reformatted for better LinkedIn engagement, while the image is fetched via HTTP request. The reformatted text and image are merged and posted to LinkedIn. Finally, the Notion entry status is updated to 'Done'.

## Output Details
The workflow publishes a formatted LinkedIn post with an image and updates the corresponding Notion database entry status to 'Done'.

## Tags
LinkedIn, Notion, OpenAI, automation, social media, scheduling, AI
