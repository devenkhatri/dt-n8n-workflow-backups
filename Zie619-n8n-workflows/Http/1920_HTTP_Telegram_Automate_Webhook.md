# Workflow Analysis for My workflow 4

## Description
Automated workflow: My workflow 4. This workflow processes data and performs automated tasks.

## Input Details
The workflow is triggered by a POST request to a webhook at `/client-feedback` and receives client feedback data.

## Process Summary
The workflow first receives client feedback via a webhook. It then prepares a prompt to ask an AI to analyze the feedback, summarize positive points, suggest improvements, and generate a social media post. This prompt is sent to an external AI service for analysis. After receiving the AI's output, the workflow parses it to extract a detailed feedback report and a social media post draft. Finally, it sends the comprehensive feedback report via email and the social media post draft to a Telegram chat.

## Output Details
The workflow produces an email containing the client feedback report and sends a social media post draft to a specified Telegram chat.

## Tags
automation,n8n,production-ready,excellent,optimized
