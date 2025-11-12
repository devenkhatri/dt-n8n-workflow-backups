# Workflow Analysis for Discord Agent

## Description
An AI-powered Discord bot that automatically responds to messages or executes tasks triggered by other workflows, formatting responses in stylish Discord text and posting to specific channels like 'ai-tools' or 'free-guides'.

## Input Details
The workflow is triggered either by another workflow passing a 'Task' input or by a direct chat message received via a Discord webhook.

## Process Summary
The workflow starts with one of two triggers: execution from another workflow (with a task) or a received Discord message. It then uses an AI agent with a system prompt that enforces Discord formatting and a 1800-character limit. The OpenAI model (gpt-4o-mini) generates a response using context from a window buffer memory. Based on the AI's output, the workflow selects the appropriate Discord channel ('ai-tools' or 'free-guides') and sends the message using configured Discord bot credentials.

## Output Details
The workflow sends a styled, AI-generated message to either the 'ai-tools' or 'free-guides' Discord channel in the specified server.

## Tags
Discord, AI Agent, OpenAI, automation, chatbot, n8n, production-ready, workflow-trigger, chat-trigger, message formatting
