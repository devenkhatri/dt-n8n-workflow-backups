# Workflow Analysis for Cocktail Recipe Sharing

## Description
This workflow automatically fetches a cocktail recipe once a week and shares it as a beautifully designed image in a Rocket.Chat channel.

## Input Details
The workflow is triggered automatically every Friday at 6 PM UTC via a cron schedule.

## Process Summary
The workflow starts with a scheduled trigger every Friday at 6 PM. It then makes an HTTP request to fetch a random cocktail recipe from an external API. Using the retrieved drink name and instructions, it generates a custom image via Bannerbear that includes the cocktail title and recipe. Finally, the generated image is posted to a configured Rocket.Chat channel.

## Output Details
The workflow posts a custom-generated cocktail recipe image to a Rocket.Chat channel every Friday.

## Tags
automation, n8n, production-ready, cocktail, recipe, bannerbear, rocketchat, scheduled, api-integration
