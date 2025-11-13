# Workflow Analysis for Automate LinkedIn Posts with AI

## Description
This workflow automatically generates and posts content on LinkedIn using AI, fetching post details from Notion.

## Input Details
The workflow is triggered daily at 3 PM and retrieves post content and associated images from a Notion database.

## Process Summary
The workflow is triggered daily at 3 PM to check for new posts in a Notion database. It retrieves the post's text content and image URL from the Notion page. The text content is then sent to an OpenAI assistant for reformatting to enhance LinkedIn engagement. Simultaneously, the associated image is fetched via an HTTP request. Finally, the reformatted text and the image are combined and posted to LinkedIn, and the post's status in Notion is updated to "Done".

## Output Details
The workflow publishes reformatted content and an image to LinkedIn and updates the status of the original post in Notion.

## Tags
automation, LinkedIn, AI, Notion, scheduled posting
