# Workflow Analysis for Amazon Ads AI Optimization

## Description
This workflow automatically analyzes Amazon Sponsored Products advertising reports using AI to generate actionable bid, budget, and targeting recommendations for performance optimization.

## Input Details
The workflow is triggered manually (or can be scheduled) and pulls Amazon Ads report files (.xlsx or .csv) from a specified Google Drive folder.

## Process Summary
The workflow first lists files in a Google Drive folder and filters for .xlsx or .csv reports. It downloads each file, preserves the original filename, and extracts tabular data accordingly. All reports are merged and categorized (search terms, campaigns, targeting, etc.) based on filename patterns. This structured data is then passed to an AI model (GPT-4o) with specific instructions to generate optimization recommendations in JSON format. Finally, the AI's output is formatted into a rich HTML email and sent to a configured recipient.

## Output Details
The workflow sends a detailed HTML email with AI-generated Amazon Ads optimization instructions, including campaign adjustments, keyword suggestions, and targeting recommendations.

## Tags
amazon ads, ai optimization, google drive, openai, gpt-4o, advertising automation, csv processing, xlsx processing, email automation, n8n
