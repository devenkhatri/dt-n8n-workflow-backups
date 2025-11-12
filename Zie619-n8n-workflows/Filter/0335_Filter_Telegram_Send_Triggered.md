# Workflow Analysis for Telegram Workflow (De)Activator

## Description
This workflow allows users to remotely activate or deactivate specific n8n workflows by sending commands via Telegram, enabling quick response to issues without needing direct access to the n8n interface.

## Input Details
The workflow is triggered by incoming Telegram messages sent to a configured bot, and it receives the message text and chat ID as input.

## Process Summary
The workflow first receives a message from Telegram and filters it to ensure it comes from an authorized chat. It then checks if the message starts with '/start' or '/stop'. Based on the command, it routes the message to the appropriate branch. The workflow then checks whether the message contains keywords like 'marketing' or 'sales' to determine which workflow to act on. Finally, it either activates or deactivates the corresponding n8n workflow using the n8n API.

## Output Details
The workflow sends an API request to the n8n instance to either activate or deactivate a specified workflow based on the Telegram command received.

## Tags
telegram, workflow management, automation, remote control, n8n api, deactivate workflow, activate workflow
