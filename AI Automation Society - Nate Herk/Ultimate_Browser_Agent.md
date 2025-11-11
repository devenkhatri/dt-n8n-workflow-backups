# Workflow Analysis for Ultimate Browser Agent

## Description
An AI-powered browser automation workflow that can navigate websites, interact with elements (click, type), extract information, and complete web-based tasks autonomously based on user requests received via chat.

## Input Details
The workflow is triggered either by a chat message from a user or by being executed from another workflow with URL and profile name inputs.

## Process Summary
The workflow starts by initializing a browser session using the Start Browser tool. It then uses an AI agent powered by Claude 3.5 Sonnet to process user requests, which can include loading URLs, typing text, clicking elements, and querying page content. The agent maintains memory of interactions and uses browser tools with session and window IDs to perform actions. Upon task completion, it terminates the browser session. When triggered externally, it also posts a live view URL to Slack for monitoring.

## Output Details
The workflow produces extracted data or completed web interactions as requested by the user, and optionally sends a live browser session link to a Slack channel for monitoring.

## Tags
browser automation, AI agent, web scraping, Airtop, Claude AI, chat-triggered, URL navigation, element interaction, session management, Slack notification
