# Workflow Analysis for YouTube Strategist

## Description
This workflow analyzes YouTube channels and videos to extract winning title formulas, thumbnail strategies, and audience insights, then generates new high-performing video ideas based on that data.

## Input Details
The workflow is triggered by either a form submission with three YouTube channel URLs, a weekly schedule for broad niche analysis, or a daily schedule for specific niche analysis.

## Process Summary
The workflow has five main phases: 1) It analyzes top-performing videos from three submitted competitor channels, extracting power words from titles and analyzing thumbnails; 2) It scrapes top videos in a broad niche weekly to identify trends; 3) It performs daily analysis of a specific niche; 4) It scrapes comments from the user's own channel to understand audience preferences; and 5) It combines all insights to generate three new video title and thumbnail ideas tailored to the channel. All data is stored in a Google Sheet for reference and analysis.

## Output Details
The workflow outputs analyzed data and insights to multiple Google Sheets tabs and sends a Slack notification with a link to the results when the daily analysis is complete.

## Tags
youtube, content strategy, social media analysis, ai analysis, competitor research, thumbnail analysis, title optimization, content ideation, google sheets, automation
