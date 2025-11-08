# Workflow Analysis for Automate LinkedIn Posts with AI

## Description
This workflow automates the process of posting daily content to LinkedIn by fetching scheduled posts from a Notion database, enhancing them with AI, and then publishing them, finally updating their status in Notion.

## Input Details
The workflow is triggered daily at 3 PM by a schedule and retrieves post data and an image from a Notion database.

## Process Summary
The workflow is initiated daily at 3 PM. It queries a Notion database for posts scheduled for the current day. For each post, it retrieves all content blocks and any associated image URL. The post's text content is sent to an OpenAI assistant for reformatting to improve readability and engagement on LinkedIn, while the image is fetched separately. The reformatted text and the fetched image are then combined, and the combined content is published as a new post on LinkedIn. Finally, the status of the original post in the Notion database is updated to "Done".

## Output Details
The workflow publishes a reformatted text post with an image to LinkedIn and updates the status of the corresponding entry in the Notion database.
