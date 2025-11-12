# Workflow Analysis for Blog Automation TEMPLATE

## Description
An automated workflow that manages the end-to-end process of generating and publishing blog posts using AI, based on a schedule defined in Google Sheets. It supports multi-stage content creation (like idea generation, drafting, and finalizing), updates the sheet with AI-generated content, and publishes finalized posts to WordPress.

## Input Details
The workflow is triggered either manually or on an hourly schedule, and it pulls configuration and content schedule data from a Google Sheet referenced via a webhook URL.

## Process Summary
The workflow begins by loading configuration and scheduled blog post data from Google Sheets. For each scheduled item that is due, it checks the current status and determines the next action (e.g., generate idea, draft, finalize). It constructs dynamic prompts using placeholders, sends them to an LLM (via OpenRouter), and processes the AI-generated output. The results are merged back into the original row and saved to the sheet. If the action is 'publish', it formats the final content as an XML-RPC request and posts it to a WordPress site, then logs the outcome.

## Output Details
The workflow updates the Google Sheet with AI-generated content or publishing status, appends log entries for each action, and publishes blog posts to WordPress when ready.

## Tags
blog automation, AI content generation, WordPress publishing, Google Sheets integration, LLM workflow, scheduled automation, n8n, production-ready
