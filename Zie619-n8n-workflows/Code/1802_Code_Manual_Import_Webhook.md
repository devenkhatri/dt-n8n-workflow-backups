# Workflow Analysis for Tiktok Downloader

## Description
This workflow downloads TikTok videos without watermarks by extracting the original video URL from the page source and saving the file to Google Drive with public sharing enabled.

## Input Details
The workflow is triggered manually and uses a TikTok video URL provided via an environment variable (WEBHOOK_URL).

## Process Summary
The workflow starts by fetching the TikTok video page HTML along with session cookies. It then parses the HTML to extract the raw video URL from a JSON script tag embedded in the page. Using the extracted URL and cookies, it downloads the watermark-free video file. Optionally, the video is uploaded to Google Drive with a filename based on the video ID, and the file permissions are set to allow public access with a link.

## Output Details
The workflow outputs the downloaded TikTok video file and optionally uploads it to Google Drive with public sharing enabled.

## Tags
TikTok downloader, video automation, no watermark, Google Drive upload, n8n workflow, production-ready
