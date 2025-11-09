# Workflow Analysis for Day2_Social_media_Multi_Posting

## Description
This workflow takes a single social media post and automatically adapts it into platform-specific versions for LinkedIn, Twitter/X, and Facebook, then saves all versions to a Google Sheet for review or scheduling.

## Input Details
The workflow is triggered manually and receives a raw social media post along with an associated topic via an embedded code node.

## Process Summary
The workflow starts by accepting an original post and topic. It then uses OpenAI's GPT model to reformat the post specifically for LinkedIn, Twitter/X, and Facebook, following each platform's best practices. Each formatted post is processed to finalize hashtags, structure, and character counts. The processed posts are combined into a single data object, and a preview of all versions is generated. Finally, the original post and all platform-specific versions are saved to a Google Sheet with a timestamp and status.

## Output Details
The workflow outputs a row in a Google Sheet containing the original post, adapted posts for LinkedIn, Twitter, and Facebook, along with timestamps and status.

## Tags
social media, content repurposing, OpenAI, Google Sheets, multi-platform posting, automation
