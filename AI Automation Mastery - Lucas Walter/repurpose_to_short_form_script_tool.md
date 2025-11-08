# Workflow Analysis for Content - Short Form AI News Script Generator

## Description
This workflow automates the process of identifying trending AI news stories, curating them for viral potential on social media, and generating engaging short-form video scripts. It combines content from markdown articles and tweets, applies an AI model to select the most impactful stories with compelling hooks, and then uses another AI to craft ready-to-use video scripts, delivering all insights and scripts to a designated Slack channel.

## Input Details
This workflow can be triggered either automatically on a daily schedule at 7 PM or manually with an optional date input to process content for a specific day.

## Process Summary
First, the workflow retrieves markdown articles and tweets from an S3 bucket for a specified date, filtering for relevant content and excluding newsletters. It then combines all collected text and metadata into a single input for an AI model. This AI analyzes the content, selects 3-5 top stories based on virality criteria, generates titles, summaries, and 2-3 unique hook angles for each. Subsequently, for each chosen story, it scrapes additional context from source URLs. Finally, a second AI model crafts two distinct 50-60 second short-form video scripts per story based on the curated content and scraped data.

## Output Details
The workflow outputs a curated list of top AI news stories, including their titles, summaries, viral hook angles, and source URLs, along with two generated video scripts for each story, all shared to a specific Slack channel for review.
