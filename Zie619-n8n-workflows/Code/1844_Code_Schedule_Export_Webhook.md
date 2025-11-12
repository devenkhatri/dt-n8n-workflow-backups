# Workflow Analysis for Backup Squarespace code Injections to Github

## Description
This workflow automatically backs up Squarespace website header and footer code injections to a GitHub repository, keeping a versioned history of custom code snippets for safekeeping and recovery.

## Input Details
The workflow is triggered either manually or automatically every 2 hours via a schedule trigger, and it receives the Squarespace website URL from an environment variable or configuration.

## Process Summary
The workflow fetches Squarespace page context data via an HTTP request, extracts header and footer code injections, and cleans them using custom JavaScript logic to remove unnecessary elements. It then formats the cleaned code with metadata like domain and timestamp, and attempts to update the corresponding file in a GitHub repository. If the file doesn’t exist, it creates a new one. The process handles errors gracefully, including cases where the Squarespace page is not found.

## Output Details
The cleaned header and footer code injections are saved as separate HTML files in a specified GitHub repository under a domain-specific folder, with a descriptive commit message including the backup timestamp.

## Tags
squarespace, github, backup, code injection, automation, n8n, production-ready
