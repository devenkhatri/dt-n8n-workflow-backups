# Workflow Analysis for Blotato Scheduled Posting

## Description
This workflow automates the creation and posting of social media content to LinkedIn, Facebook, and Instagram based on a schedule.

## Input Details
This workflow is triggered every weekday (Monday to Friday) by a CRON schedule.

## Process Summary
The workflow starts by retrieving pre-written content from Google Sheets. It then uses OpenAI to generate an image based on the content. The image is cropped using an external API and uploaded to Google Drive. Finally, the workflow posts the content and the generated image to LinkedIn, Facebook, and Instagram.

## Output Details
The workflow posts content to LinkedIn, Facebook, and Instagram and saves the generated image to Google Drive.
