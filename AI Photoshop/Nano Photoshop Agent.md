# Workflow Analysis for Nano Photoshop Agent

## Description
This workflow creates a Telegram-based AI assistant that can handle photo uploads, store them in Google Drive, and perform various image operations like renaming, editing, combining images, and searching through stored files using natural language commands.

## Input Details
The workflow is triggered by messages sent to a Telegram bot, which can contain either text commands or photo uploads.

## Process Summary
When a user sends a message to the Telegram bot, the workflow first checks if it contains a photo or text. If a photo is received, it downloads the image, uploads it to a designated Google Drive folder, and informs the AI agent. The AI agent (powered by either Anthropic's Claude or OpenAI's GPT) processes the user's text requests using available tools to perform actions like renaming files, combining images, editing images, or searching through stored files. The agent maintains conversation memory per user and sends responses back to the Telegram chat.

## Output Details
The workflow sends responses back to the Telegram chat with results of the AI agent's actions, such as confirmation messages, file links, or answers to user queries.

## Tags
telegram, google drive, image processing, AI agent, file management, Claude, GPT, image editing, workflow automation
