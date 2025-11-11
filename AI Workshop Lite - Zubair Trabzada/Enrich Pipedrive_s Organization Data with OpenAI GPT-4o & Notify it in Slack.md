# Workflow Analysis for piepdrive-test

## Description
This workflow automatically enriches newly created Pipedrive organization records by scraping their website content, summarizing key business information using GPT-4o, and adding the summary as a note in Pipedrive while also sending a formatted notification to Slack.

## Input Details
The workflow is triggered when a new organization is created in Pipedrive and receives the organization data including a custom website field.

## Process Summary
When a new organization is created in Pipedrive, the workflow extracts the organization's website URL and uses ScrapingBee to fetch its HTML content. This content is sent to OpenAI's GPT-4o model with instructions to generate a structured HTML summary including company description, target market, unique selling points, and potential competitors. The generated HTML summary is saved as a note attached to the Pipedrive organization. The HTML is then converted to Markdown and reformatted into Slack-compatible Markdown before being posted to a designated Slack channel.

## Output Details
The workflow creates a detailed HTML note in Pipedrive for the new organization and sends a Slack message with the same information formatted for Slack.

## Tags
pipedrive, openai, gpt-4o, web scraping, slack, crm enrichment, automation
