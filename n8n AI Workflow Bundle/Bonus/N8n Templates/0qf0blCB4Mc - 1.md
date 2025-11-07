# Workflow Analysis for Automated Faceless AI Video Creation and Social Media Publishing

## Description
This workflow automates the creation of faceless AI videos based on historical facts and publishes them to multiple social media platforms.

## Input Details
The workflow is triggered daily at 10 AM by a schedule.

## Process Summary
First, an AI agent brainstorms viral video ideas, selects one, researches facts, and generates a 15-second video script and a short caption. Next, the workflow prepares parameters for video creation using the Blotato API, including the script, voice, and visual style. It then initiates the video creation process and waits for 10 minutes for the video to be processed. Once the video is ready, its URL is retrieved, and it is uploaded to Blotato's media library. Finally, the video and its caption are published to Instagram, Facebook, LinkedIn, and Threads using the Blotato API.

## Output Details
The workflow publishes the generated AI video and its corresponding caption to Instagram, Facebook, LinkedIn, and Threads.
