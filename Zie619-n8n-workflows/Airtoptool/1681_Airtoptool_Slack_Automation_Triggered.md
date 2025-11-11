# Workflow Analysis for Airtop Web Agent

## Description
This workflow enables users to instruct an AI-powered web agent to perform tasks on websites, such as navigating pages, clicking elements, typing text, and extracting information. It supports authentication via Airtop profiles and returns a summary of the results.

## Input Details
The workflow is triggered by a form submission where the user provides a natural language prompt and optionally an Airtop profile name for authenticated sites.

## Process Summary
The workflow starts by capturing user instructions via a form. An AI agent (Claude 3.5 Haiku) interprets the prompt and orchestrates browser actions using Airtop tools: starting a browser session, loading a URL, querying page content, clicking elements, and typing text as needed. Once the task is complete, the session is terminated, and the AI synthesizes the results into a structured output. Optionally, the workflow can send the Live View URL and final output to a Slack channel for monitoring.

## Output Details
The workflow outputs a synthesized summary of the AI agent's findings and actions, and optionally posts the browser Live View URL and result to a Slack channel.

## Tags
AI agent, web automation, Airtop, browser automation, form trigger, Claude AI, Slack integration, no-code automation, production-ready, web scraping
