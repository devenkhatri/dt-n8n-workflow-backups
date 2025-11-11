# Workflow Analysis for Dynamic Models

## Description
This workflow intelligently selects the best AI model for a given user request and executes the appropriate actions—such as creating calendar events, drafting emails, searching the web, or answering policy questions using a company knowledge base—then logs the interaction and responds back to the user.

## Input Details
The workflow is triggered by either a Slack message mentioning the bot or a direct chat message via a chat interface, containing the user's natural language request.

## Process Summary
First, a model selector agent analyzes the user's request and picks the most suitable AI model based on task type. Then, a 'Smarty Pants' agent uses the selected model along with access to tools (Gmail, Google Calendar, Airtable contacts, and Tavily web search) to fulfill the request. In parallel, a separate RAG (Retrieval-Augmented Generation) flow handles policy/FAQ queries by consulting a Supabase vector knowledge base. All interactions are logged to a Google Sheet with timestamp, input, output, and model used. Finally, the response is sent back to the Slack channel or chat interface.

## Output Details
The workflow sends a response to Slack or the chat interface, logs the interaction in a Google Sheet, and may trigger side effects like creating a calendar event, drafting an email, or retrieving information from a knowledge base or web search.

## Tags
AI agent, dynamic model selection, Slack integration, RAG, knowledge base, tool calling, Google Workspace, Airtable, Tavily, logging
