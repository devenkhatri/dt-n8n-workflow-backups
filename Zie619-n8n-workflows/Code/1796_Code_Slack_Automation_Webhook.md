# Workflow Analysis for piepdrive-test

## Description
This workflow automatically enriches newly created Pipedrive organization records by scraping their website, using AI to generate a detailed summary, and then adding that summary as a note in Pipedrive while also sending a formatted notification to Slack.

## Input Details
The workflow is triggered when a new organization is created in Pipedrive and receives the organization’s data, including a custom website field.

## Process Summary
When a new organization is created in Pipedrive, the workflow scrapes the organization's website using a scraping API. The scraped HTML content is sent to OpenAI’s GPT-4o model, which generates a structured HTML summary including company description, target market, unique selling points, and potential competitors. This summary is added as a note to the organization in Pipedrive. The HTML is then converted to Markdown and further formatted into Slack-compatible Markdown before being sent as a message to a designated Slack channel.

## Output Details
The workflow creates a rich note in Pipedrive for the new organization and sends a formatted summary message to a Slack channel.

## Tags
Pipedrive, OpenAI, GPT-4o, web scraping, Slack integration, CRM automation, AI enrichment, organization onboarding
