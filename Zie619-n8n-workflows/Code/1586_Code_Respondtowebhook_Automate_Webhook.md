# Workflow Analysis for Youtube Discord Bot

## Description
This workflow powers a Discord bot that answers user questions using AI, with special knowledge of the Presting Podcasts YouTube channel transcripts. It receives questions from Discord users via a webhook, processes them using Google Gemini AI, and returns a properly formatted response mentioning the user.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint containing Discord user data, including the username and their question.

## Process Summary
The workflow starts by receiving a question and username from Discord via a webhook. It constructs a prompt for an AI model, incorporating context about the Presting Podcasts YouTube channel. The Google Gemini AI model generates a response in the language of the original question. A code node formats the AI's output into a Discord-friendly message that mentions the user. Finally, the formatted response is sent back through the webhook to Discord.

## Output Details
The workflow returns a JSON response containing the AI-generated answer formatted to mention the Discord user, which is sent back to Discord via the webhook.

## Tags
Discord bot, YouTube, AI assistant, Google Gemini, webhook, automation, n8n, production-ready
