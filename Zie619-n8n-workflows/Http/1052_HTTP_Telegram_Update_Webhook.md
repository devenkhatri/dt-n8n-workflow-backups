# Workflow Analysis for Receive updates from Telegram and send an image of a cocktail

## Description
This workflow listens for incoming messages on Telegram and automatically replies with an image and name of a cocktail fetched from an external API.

## Input Details
The workflow is triggered by any new message sent to a Telegram bot.

## Process Summary
When a message is received via Telegram, the workflow makes an HTTP request to a predefined cocktail API endpoint (configured via the BASE_URL environment variable). It extracts the first cocktail's image URL and name from the API response. Then, it sends a photo message back to the Telegram chat with the cocktail image, captioned with the drink's name, and replies directly to the original user message.

## Output Details
The workflow sends a photo message with a cocktail image and name back to the Telegram chat where the original message was received.

## Tags
Telegram, cocktail, API integration, automation, n8n, production-ready
