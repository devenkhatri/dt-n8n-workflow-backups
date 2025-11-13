# Workflow Analysis for Github Releases

## Description
This workflow automatically monitors specified GitHub repositories for new releases, processes their content using AI for extraction and translation, and sends notifications to a Slack channel.

## Input Details
The workflow is triggered hourly by a cron schedule, and it uses a predefined list of GitHub repositories as its initial data input.

## Process Summary
The workflow starts by fetching a list of configured GitHub repositories. For each repository, it attempts to read its release RSS feed. If an error occurs during the RSS fetch, a Slack error notification is sent. Otherwise, it retrieves the last processed release ID from Redis and compares it with the latest fetched release. If a new release is detected, its content is processed by a Gemini AI model to extract and translate key information (features, fixes, others) into Chinese. The processed information is then formatted into a structured Slack message and sent to a dedicated Slack channel, while the new release ID is simultaneously stored in Redis.

## Output Details
The workflow sends detailed release notifications to a Slack channel and updates a Redis database with the ID of the latest processed release for each monitored repository.

## Tags
automation,n8n,production-ready,excellent,optimized,github,releases,slack,redis,ai,gemini,notification
