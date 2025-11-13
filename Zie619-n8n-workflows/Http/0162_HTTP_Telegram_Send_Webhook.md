# Workflow Analysis for Daily Vegan Recipe Telegram Bot

## Description
This workflow powers a Telegram bot that sends a daily vegan recipe to subscribed users. It also automatically welcomes new users, saves their chat details to Airtable, and ensures each user receives one recipe per day.

## Input Details
The workflow is triggered either by a scheduled cron job (for daily recipe delivery) or by new messages to a Telegram bot (for welcoming new users).

## Process Summary
When triggered by a cron job, the workflow fetches user chat IDs from Airtable, retrieves a random vegan recipe from an external API, and sends the recipe image and URL to each user via Telegram. Separately, when a new user messages the Telegram bot, the workflow sends a welcome message, records the user’s chat ID and name in Airtable (if not already present), and immediately sends them their first recipe.

## Output Details
The workflow sends recipe images and links to Telegram users and stores new user data in an Airtable database.

## Tags
telegram bot, recipe automation, daily reminder, airtable integration, cron job, user onboarding, vegan recipes, n8n workflow
