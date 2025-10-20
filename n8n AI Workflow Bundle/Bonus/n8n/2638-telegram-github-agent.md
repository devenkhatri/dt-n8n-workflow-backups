# Workflow Analysis for Telegram Github Agent

## Description
This workflow converts voice messages from Telegram into text, which is then used as a prompt for an AI to generate a GitHub issue description. Finally, it creates a new GitHub issue with the generated description.

## Input Details
The workflow is triggered by an incoming voice message to a Telegram bot.

## Process Summary
The workflow starts by receiving a new voice message from Telegram. It then downloads the voice message and converts it into text using an AI model. This text is then used as a prompt for another AI model to generate a detailed GitHub issue description. Finally, a new GitHub issue is created with the generated description.

## Output Details
The workflow creates a new GitHub issue with the AI-generated description.
