# Workflow Analysis for Blog Automation TEMPLATE

## Description
This workflow automates the end-to-end process of generating, refining, and publishing blog posts using AI. It reads scheduled tasks and configuration from a Google Sheet, uses an LLM (via OpenRouter) to generate or update content based on customizable prompts, saves intermediate and final content back to the sheet, and automatically publishes completed posts to a WordPress site via XML-RPC.

## Input Details
The workflow is triggered either manually or on an hourly schedule, and it pulls configuration and scheduled blog post tasks from a Google Sheet.

## Process Summary
The workflow starts by loading settings, configuration, and scheduled blog tasks from a Google Sheet. For each scheduled task that is due and has a pending action, it retrieves a corresponding AI prompt from the config and sends it to an LLM to generate content. The AI output is cleaned, merged with existing row data, and saved back to the Google Sheet. If the action is 'publish' and the scheduled time has passed, the workflow formats the post and publishes it to WordPress using XML-RPC. All steps are logged to a 'Log' sheet, and successful publishes update the post status in the schedule sheet.

## Output Details
The workflow updates the Google Sheet with generated content and status changes, logs all actions to a dedicated log sheet, and publishes completed blog posts to a WordPress site.

## Tags
blog automation, AI content generation, WordPress publishing, Google Sheets integration, LLM, OpenRouter, scheduled publishing, content workflow
