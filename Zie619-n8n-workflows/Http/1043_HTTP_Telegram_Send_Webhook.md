# Workflow Analysis for Send a cocktail recipe every day via a Telegram

## Description
This workflow automatically sends a daily cocktail recipe with an image and instructions to a specified Telegram chat every evening at 8 PM UTC.

## Input Details
The workflow is triggered daily at 8 PM UTC by a cron scheduler and fetches cocktail recipe data from an external API endpoint defined in the environment variable BASE_URL.

## Process Summary
The workflow starts with a Cron trigger set to run daily at 8 PM UTC. It then makes an HTTP request to a predefined API endpoint to fetch a random cocktail recipe. The response includes details like the drink name, image URL, and instructions. The workflow sends this information to a Telegram chat using a Telegram bot, including the drink image and instructions as a caption. If any step fails, the workflow stops and returns an error message via the Error Handler node.

## Output Details
The workflow sends a photo message with cocktail instructions to a Telegram chat using a configured Telegram bot.

## Tags
automation, telegram, cron, cocktail, recipe, daily, notification, n8n, production-ready, api-integration
