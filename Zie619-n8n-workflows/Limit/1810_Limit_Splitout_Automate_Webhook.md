# Workflow Analysis for 🔥📈🤖 AI Agent for n8n Creators Leaderboard - Find Popular Workflows

## Description
Automated workflow: 🔥📈🤖 AI Agent for n8n Creators Leaderboard - Find Popular Workflows. This workflow integrates 19 different services: convertToFile, stickyNote, merge, lmChatOpenAi, chatTrigger. It contains 50 nodes and follows best practices for error handling and security.

## Input Details
The workflow is triggered either by a chat message containing a username (e.g., "show me stats for username joe") or by another workflow providing a username as input.

## Process Summary
The workflow starts by setting global variables and then fetches aggregated creator and workflow statistics via HTTP requests from a base URL. It parses the retrieved data, splits it into individual items, sorts them by weekly inserters, and limits them to the top 25 creators and top 300 workflows. The creator and workflow data are then merged based on the username and filtered to focus on the specific creator from the input. Finally, an AI agent generates a comprehensive Markdown report from the filtered data, which is then converted into a file and saved locally.

## Output Details
The workflow produces a comprehensive Markdown report about a specific n8n community workflow contributor, which is saved locally as a file.

## Tags
automation, n8n, production-ready, excellent, optimized
