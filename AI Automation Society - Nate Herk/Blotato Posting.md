# Workflow Analysis for Blotato Posting

## Description
This workflow automatically posts content to multiple social media platforms using Blotato based on entries in a Google Sheet that are marked as 'Ready To Post'.

## Input Details
The workflow is triggered on a schedule and pulls data from a Google Sheet where rows have a 'Status' of 'Ready To Post'.

## Process Summary
The workflow starts by fetching a row from a Google Sheet marked as 'Ready To Post'. It extracts the Google Drive ID from the media URL and uploads the media to Blotato. The uploaded media is then simultaneously posted to Instagram, TikTok, Bluesky, Facebook, LinkedIn, Pinterest, Threads, X (Twitter), and YouTube using the title and caption from the sheet. If successful, the row's status is updated to 'Posted'; if an error occurs during upload, the status is updated to 'Errored'.

## Output Details
The workflow posts content to nine different social media platforms via Blotato and updates the corresponding row in the Google Sheet to reflect whether the post was successful ('Posted') or failed ('Errored').

## Tags
social media automation, Blotato, Google Sheets, scheduled posting, multi-platform posting
