# Workflow Analysis for YouTube Channel to Telegram Monitor

## Description
This workflow monitors a specified YouTube channel for new video uploads and sends a notification with the video details to a Telegram chat.

## Input Details
This workflow is triggered every 5 minutes by a CRON schedule.

## Process Summary
First, the workflow checks a YouTube channel for new videos. Then, it filters out any videos that have already been processed to avoid duplicate notifications. For each new video, it constructs a message containing the video title and URL. Finally, it sends these messages to a designated Telegram chat.

## Output Details
The workflow sends new YouTube video notifications to a Telegram chat.
