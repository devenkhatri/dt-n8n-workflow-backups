# Workflow Analysis for Automatically Update YouTube Video Descriptions with Inserted Text

## Description
This workflow helps YouTubers automatically insert a specific line of text (like a link or announcement) between two predefined lines in the descriptions of their YouTube videos, ensuring consistent updates across multiple videos without manual editing.

## Input Details
The workflow is manually triggered and uses environment variables to define the text to insert and its placement context within video descriptions.

## Process Summary
The workflow starts by manually triggering the process, then retrieves up to 3 of the user's most recent YouTube videos. It loops through each video, fetches its full details, and uses custom JavaScript code to insert a new line of text between two specified existing lines in the description. The updated description, along with other video metadata, is then sent back to YouTube to update the video.

## Output Details
The workflow updates the description of each targeted YouTube video with the newly inserted text while preserving the rest of the content.

## Tags
YouTube, video description, automation, text insertion, content management, n8n, production-ready
