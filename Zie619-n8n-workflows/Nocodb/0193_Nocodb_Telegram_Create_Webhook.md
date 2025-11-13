# Workflow Analysis for Production Workflow

## Description
This workflow handles user interactions for a multi-language Telegram bot, managing user data and delivering appropriate responses.

## Input Details
The workflow is triggered by incoming messages from a Telegram bot.

## Process Summary
The workflow is activated by a Telegram message. It loads a multi-language message dictionary and determines the user's chat ID and preferred language. It checks if the user is new or returning by querying a NocoDB database. Based on the user's status and message content, it routes the interaction to send a localized greeting, welcome-back, help, or error message. New users are recorded, and existing users' language preferences are updated in NocoDB.

## Output Details
The workflow sends localized messages to the Telegram user and updates a NocoDB database with user information (chat ID and last used language).

## Tags
automation, n8n, production-ready, excellent, optimized
