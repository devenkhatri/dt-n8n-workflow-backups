# Workflow Analysis for Confluence Knowledge Base Search Workflow

## Description
This workflow enhances IT support by searching a Confluence knowledge base in response to user queries received from a parent AI agent workflow. It retrieves relevant articles and formats a structured response including the title, link, and excerpt to be used in a final AI-generated reply to the user.

## Input Details
The workflow is triggered by a parent workflow and receives a user query as input via the Execute Workflow Trigger node.

## Process Summary
The workflow starts by receiving a user query from a parent workflow. It then sends this query to Confluence’s API using an HTTP request with CQL (Confluence Query Language) to search for matching content. The response from Confluence is processed to extract the title, web link, and excerpt of the top result. This information is formatted into a structured response object. Finally, the formatted response is passed back to the parent workflow for use in generating a user-facing answer.

## Output Details
The workflow outputs a structured response containing the article title, URL, and excerpt, which is returned to the parent workflow for inclusion in an AI-generated message to the user.

## Tags
Confluence, knowledge base, AI agent, IT support, Slack integration, search, automation, n8n
