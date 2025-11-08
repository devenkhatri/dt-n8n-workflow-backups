# Workflow Analysis for Content - Short Form News Script Generator

## Description
This workflow automates the process of identifying trending AI news, generating engaging short-form video scripts, and sharing them on Slack for content creators.

## Input Details
The workflow is triggered either on a daily schedule or manually with an optional input date, which determines the news content to be processed.

## Process Summary
The workflow begins by collecting daily AI news content from an S3 bucket, encompassing both markdown articles and tweets, and then filters this data. This curated content is then fed to an AI model to identify 3-5 top stories, generating engaging titles, concise summaries, and viral hook angles for each. For every selected story, the workflow proceeds to scrape additional context from its associated source URLs. Finally, a second AI model crafts two distinct 50-60 second video scripts per story, designed for short-form video platforms.

## Output Details
The workflow publishes an initial message, the curated stories with their potential hooks and sources, and the generated video scripts to a designated Slack channel.
