# Workflow Analysis for Build your first AI MCP Server

## Description
This workflow demonstrates how to build an AI-powered Model Context Protocol (MCP) server that can handle natural language requests to perform various tasks like managing Google Calendar events, converting text case, generating random user data, and fetching jokes. It uses an AI agent to interpret user requests and route them to the appropriate tools.

## Input Details
The workflow is triggered by chat messages or HTTP requests (via MCP triggers) containing natural language instructions that the AI agent processes.

## Process Summary
The workflow starts with an AI agent that receives natural language requests. Based on the request, it routes to either a Calendar MCP server (for calendar operations like search, create, update, delete events) or a Functions MCP server (for text conversion, random data generation, and joke fetching). The Functions MCP uses a switch node to determine which function to execute (uppercase, lowercase, random user data, or jokes) and processes the input accordingly. Results are formatted and returned to the user.

## Output Details
The workflow returns processed results such as calendar event modifications, converted text, generated user data, or jokes back to the user via the AI agent or HTTP response.

## Tags
AI, MCP, Google Calendar, text processing, automation, n8n, production-ready
