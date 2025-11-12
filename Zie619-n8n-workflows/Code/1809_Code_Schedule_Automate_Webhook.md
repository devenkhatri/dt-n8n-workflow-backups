# Workflow Analysis for Blog Automation TEMPLATE

## Description
This workflow automates the end-to-end process of blog content creation and publishing. It reads scheduled tasks and configuration from a Google Sheet, uses an AI language model to generate or refine content (like titles, drafts, or final posts), updates the sheet with the generated content, and automatically publishes finalized posts to a WordPress blog via XML-RPC. All actions and publishing results are logged back to the sheet for tracking.

## Input Details
The workflow is triggered either manually or on an hourly schedule, and it pulls data from a Google Sheet containing blog post tasks and configurations.

## Process Summary
The workflow begins by loading settings and fetching configuration and scheduled blog tasks from Google Sheets. For each scheduled row, it checks if the scheduled time has passed and if an action (like generating a draft or publishing) needs to be performed. If so, it constructs a dynamic AI prompt using placeholders, sends it to an LLM via a configured model, and processes the response. The generated content is merged with existing data and saved back to the sheet. If the action is 'publish', it formats the post as XML and sends it to WordPress, then logs success or failure.

## Output Details
The workflow updates the Google Sheet with AI-generated content and publishing status, logs all operations to a dedicated log sheet, and publishes finalized blog posts to a WordPress site.

## Tags
blog automation, AI content generation, WordPress publishing, Google Sheets integration, scheduled workflow, LLM, n8n, production-ready
