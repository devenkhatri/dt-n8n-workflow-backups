# Workflow Analysis for NeurochainAI Basic API Integration

## Description
An automated workflow that integrates with NeurochainAI's API to provide AI-powered text and image generation capabilities directly through Telegram.

## Input Details
The workflow is triggered by messages received from a connected Telegram bot.

## Process Summary
The workflow starts by receiving a Telegram message and sending a "typing" action and a "⌛" emoji. It then checks the message content to determine if it's a command for text generation, image generation, or a general query. Based on this, it makes a corresponding API call to either the "NeurochainAI - REST API" for text or the "NeurochainAI - Flux" for image generation. The messages are cleaned by removing prefixes before being sent to the AI APIs. After receiving a response, it handles potential errors or sends the generated content back to the user. Finally, it deletes the initial "⌛" status message.

## Output Details
The workflow sends AI-generated text responses or images, along with status and error messages, back to the originating Telegram chat.

## Tags
Telegram, AI, Text Generation, Image Generation, Automation, n8n, API Integration, Error Handling, Production-ready
