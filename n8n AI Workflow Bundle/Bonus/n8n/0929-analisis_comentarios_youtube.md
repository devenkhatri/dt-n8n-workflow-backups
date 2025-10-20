# Workflow Analysis for YouTube Comment Analysis and Labeling

## Description
This workflow automates the analysis of YouTube video comments by fetching comments, analyzing their sentiment and category using AI, and then labeling them in a Google Sheet. It allows for efficient processing and categorization of user feedback on YouTube.

## Input Details
The workflow is triggered manually and requires a YouTube video ID as input.

## Process Summary
The workflow starts by retrieving all comments from the specified YouTube video. It then prepares these comments for AI processing by combining the author and comment text. Each comment is then sent to an AI model to determine its sentiment and category. Finally, the original comment, its sentiment, and its category are added as a new row to a Google Sheet.

## Output Details
The workflow outputs the processed comments, their sentiment, and their category into a specified Google Sheet.
