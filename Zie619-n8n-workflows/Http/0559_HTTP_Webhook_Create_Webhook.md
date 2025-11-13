# Workflow Analysis for Create Confluence Page from Template

## Description
This workflow automatically creates a new page in Atlassian Confluence by fetching a space template, replacing placeholders in the title and body with dynamic data, and publishing it to a specified space and parent page.

## Input Details
The workflow is triggered by a POST webhook request that includes JSON data containing values to replace placeholders in the Confluence template.

## Process Summary
The workflow starts with a webhook that receives dynamic data. It then sets fixed parameters like template ID, target space key, and parent page ID. Next, it fetches the content of a Confluence template using an HTTP request. A code node processes the template by replacing placeholders (e.g., $user.name$) with values from the webhook payload. Finally, it sends another HTTP request to Confluence to create a new page with the updated title and body in the specified location.

## Output Details
The workflow creates a new page in Atlassian Confluence with a dynamically generated title and body, placed under a designated parent page in a specified space.

## Tags
Confluence, Atlassian, template, automation, webhook, page creation, placeholder replacement, n8n, production-ready
