# Workflow Analysis for N8N Español - NocodeBot

## Description
A Telegram bot that responds to user queries about no-code tools by fetching descriptions from a Strapi database, translating them into the user's language, and sending back the translated description along with an associated image.

## Input Details
The workflow is triggered by messages sent to a Telegram bot, particularly responding to tool names or the /start command.

## Process Summary
When a user sends a message to the Telegram bot, the workflow checks if it's the /start command and sends a welcome message. If it's a tool name, it fetches matching data from a Strapi API, retrieves the tool's image and description, translates the description into the user's Telegram language using a command-line translation tool, and sends both the image and translated description back to the user via Telegram.

## Output Details
The workflow sends a translated tool description and associated image back to the user in Telegram, or a welcome message if the user sends /start.

## Tags
Telegram bot, no-code tools, translation, Strapi integration, automation, n8n, production-ready
