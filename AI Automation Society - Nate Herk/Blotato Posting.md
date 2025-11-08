# Workflow Analysis for Blotato Social Media Content Posting

## Description
This workflow automates the process of publishing social media content. It periodically checks a Google Sheet for new posts marked "Ready To Post", uploads the associated media, distributes the content across nine different social media platforms, and then updates the Google Sheet with the posting status.

## Input Details
The workflow is triggered by a schedule and reads content data from a Google Sheet.

## Process Summary
The workflow starts on a schedule, retrieves content with a "Ready To Post" status from a Google Sheet, extracts the Google Drive ID from the media URL, and then uploads the media to Blotato. Subsequently, it posts the content (title, caption, and uploaded media) to Instagram, TikTok, Bluesky, Facebook, LinkedIn, Pinterest, Threads, X, and YouTube. If the posting is successful, it updates the Google Sheet status to "Posted"; otherwise, it marks the status as "Errored".

## Output Details
The workflow posts content to various social media platforms and updates the status in a Google Sheet.
