# Workflow Analysis for YouTube Videos with AI Summaries on Discord

## Description
This workflow automatically detects new videos on a specified YouTube channel, retrieves their English captions, generates a concise three-bullet point summary using ChatGPT, and then posts this information, along with the video link, to a Discord channel.

## Input Details
The workflow is triggered by new video uploads detected in a specified YouTube channel's RSS feed, receiving video metadata such as title and ID.

## Process Summary
The workflow begins by monitoring a YouTube channel's RSS feed for new video uploads. Upon detection, it retrieves the video's caption data from the YouTube API, specifically looking for and downloading the English caption track. The downloaded caption content is then extracted as plain text. This text is sent to OpenAI's ChatGPT to generate a three-bullet point summary. Finally, a message containing the video title, the AI-generated summary, and a direct link to the video is posted to a Discord channel.

## Output Details
The workflow produces a formatted Discord message containing the new YouTube video's title, an AI-generated summary, and its watch link, which is then sent to a predefined Discord channel via a webhook.
