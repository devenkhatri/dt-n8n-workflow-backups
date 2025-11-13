# Workflow Analysis for Automate LinkedIn Posts with AI

## Description
This workflow automates the process of posting content to LinkedIn daily at 3 PM, leveraging AI for content refinement. It ensures that pre-scheduled posts from Notion are published on time and in an engaging format.

## Input Details
The workflow is triggered by a schedule trigger daily at 3 PM.

## Process Summary
First, the workflow queries a Notion database for LinkedIn posts scheduled for the current day. It then retrieves all content, including text and image URLs, from the selected Notion post. The text content is sent to an OpenAI assistant to be reformatted for better LinkedIn engagement. Concurrently, the associated image is fetched via an HTTP request. Finally, the reformatted text and the image are combined and posted to LinkedIn, and the status of the original post in Notion is updated to "Done".

## Output Details
The workflow publishes reformatted text and an image to LinkedIn and updates the status of the original post in a Notion database.

## Tags
automation, n8n, production-ready, excellent, optimized
