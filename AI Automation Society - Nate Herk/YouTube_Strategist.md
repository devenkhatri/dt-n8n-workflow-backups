# Workflow Analysis for YouTube Content Strategist & Analyzer

## Description
This workflow helps YouTube creators generate high-performing video ideas by analyzing niche outliers, broad and specific niche trends, and audience feedback. It uses AI to extract insights from video titles and thumbnails, and provides actionable data for content strategy.

## Input Details
This workflow is triggered manually via a form submission requiring three YouTube channel URLs, or automatically on a weekly schedule (Sundays) for broad niche analysis, and daily at 6 AM for specific niche analysis.

## Process Summary
The workflow operates in five phases: 1) **Niche Outliers:** It scrapes popular videos from user-provided YouTube channels, analyzes titles for "power words" and thumbnails for attention-grabbing elements, then saves this data to a Google Sheet. 2) **Broad Niche Insights (Weekly):** It automatically scrapes popular videos for a broad niche, analyzes them, and records insights weekly. 3) **Niche Insights (Daily):** Daily, it scrapes and analyzes popular videos for a specific niche, saving the data. 4) **Comment Analysis:** It scrapes comments from a specified YouTube channel to identify audience likes, dislikes, and content requests, storing these insights. 5) **Ideation:** Combining data from high-performing videos (titles, power words, thumbnail analysis) and audience feedback, it uses an AI agent to generate three unique YouTube video title and thumbnail ideas, which are then saved.

## Output Details
The workflow outputs detailed analysis of YouTube videos (channel, title, URL, thumbnail, views, likes, power words, thumbnail analysis), audience insights, and new video title and thumbnail ideas to various Google Sheets. It also sends a Slack notification with a link to the daily niche insights.
