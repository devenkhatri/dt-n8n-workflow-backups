# Workflow Analysis for 🔥📈🤖 AI Agent for n8n Creators Leaderboard - Find Popular Workflows

## Description
This automated n8n workflow leverages an AI agent to generate a comprehensive report on n8n community workflow creators and their popular workflows. It integrates multiple services to fetch, process, and analyze data, following best practices for error handling and security.

## Input Details
The workflow is triggered either by a chat message providing a username or by another workflow executing it with a username in the input query.

## Process Summary
The workflow initializes global variables for data sources and fetches aggregated creator and workflow statistics from GitHub via HTTP requests. It then parses, splits, sorts (top 25 creators, top 300 workflows), and assigns the data to structured fields. Creator and workflow data are merged by username, and the combined data is filtered for a specific creator. An AI agent processes this filtered data to generate a detailed Markdown report with workflow statistics and community insights. Finally, the generated Markdown report is converted to a file and saved locally with a timestamp.

## Output Details
The workflow produces a comprehensive Markdown report about a specific n8n workflow contributor and their workflows, which is then saved locally as a timestamped .md file.

## Tags
automation,n8n,production-ready,excellent,optimized
