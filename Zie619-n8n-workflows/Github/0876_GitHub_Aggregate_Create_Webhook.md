# Workflow Analysis for GitHub MCP Server for Issue Management

## Description
This workflow acts as a secure GitHub Model Context Protocol (MCP) server that allows external AI agents or clients to interact with GitHub issues—fetching the latest issues, retrieving comments on a specific issue, or adding new comments—while restricting access to only the necessary repository operations.

## Input Details
The workflow is triggered by another workflow or an MCP client and receives input parameters including the operation type (e.g., 'getLatestIssues', 'getIssueComments', 'addIssueComment'), repository name, issue number, and comment text.

## Process Summary
The workflow starts by receiving an operation request and associated parameters. A switch node routes execution based on the operation type. For 'getLatestIssues', it fetches up to 10 recent issues from the specified repository and formats them. For 'getIssueComments', it retrieves a specific issue and its comments, then simplifies the comment data. For 'addIssueComment', it posts a new comment to the specified issue. All results are aggregated and returned in a structured format.

## Output Details
The workflow outputs structured data about GitHub issues or comments, or a confirmation that a comment was added, which is sent back to the calling workflow or MCP client.

## Tags
GitHub, MCP server, issue tracking, automation, AI integration, n8n, workflow, comments, repository management
