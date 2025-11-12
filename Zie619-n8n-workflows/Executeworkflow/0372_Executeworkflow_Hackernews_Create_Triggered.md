# Workflow Analysis for AI Agent with Hacker News Custom Tool

## Description
This workflow creates an AI-powered chat agent that can respond to user questions by using a custom tool to fetch and return the top 50 most popular posts from Hacker News. For example, a user can ask 'What is the 5th most popular post ever on Hacker News?' and the agent will provide an answer using real-time data.

## Input Details
The workflow is triggered when a chat message is received via a 'When chat message received' node.

## Process Summary
The workflow starts when a user sends a message via chat. An AI agent, powered by OpenAI’s GPT-4o-mini model, interprets the message and decides whether to use a custom tool. That tool is implemented as a sub-workflow that fetches the top 50 Hacker News posts, cleans and formats the data by extracting key fields like title, points, URL, author, and date, and then returns the result as a JSON string. The AI agent uses this data to formulate a response to the user’s question.

## Output Details
The workflow enables the AI agent to return a natural language answer to the user’s chat query, based on processed Hacker News data.

## Tags
AI agent, chatbot, Hacker News, OpenAI, custom tool, data fetching, JSON processing, n8n workflow, automation, production-ready
