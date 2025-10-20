# Workflow Analysis for Hacker News Video Creator

## Description
This workflow automates the creation of short videos based on trending Hacker News stories. It fetches top articles, summarizes them using AI, converts the summaries to audio, generates corresponding images, and then compiles everything into a video for social media sharing.

## Input Details
The workflow is triggered manually.

## Process Summary
The workflow starts by fetching the top 5 articles from Hacker News. It then iterates through each article, generating a summary and relevant keywords using large language model (LLM). For each summary, it generates speech audio and creates an image based on the article title. Finally, all the generated components (summary text, audio, and images) are combined into a short video using an AI video generation tool.

## Output Details
The workflow outputs a `.mp4` video file to a specified folder on Google Drive.
