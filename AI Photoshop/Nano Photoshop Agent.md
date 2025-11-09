# Workflow Analysis for Nano Photoshop Agent

## Description
A Telegram-integrated AI assistant that manages photo uploads to Google Drive and performs AI-powered image operations like renaming, editing, combining images, and searching through stored files.

## Input Details
The workflow is triggered by messages sent to a Telegram bot, which can include either a photo or text input.

## Process Summary
When a message arrives via Telegram, the workflow checks if it contains a photo or text. If it's a photo, the image is downloaded, uploaded to a designated Google Drive folder, and a confirmation message with the file ID is prepared. Text inputs or the prepared photo confirmation are then sent to an AI-powered Photoshop Agent that uses either GPT-5-mini or Claude Sonnet 3.5 as its reasoning engine. The agent can perform various actions using connected tools, including renaming files in Google Drive, combining two images, editing images with AI, or searching through raw or AI-generated image libraries in Google Drive. The agent's response is sent back to the user via Telegram.

## Output Details
The workflow sends a response message back to the user in Telegram, which may include a file ID confirmation or results from AI-powered image operations.

## Tags
Telegram, Google Drive, AI Agent, Image Editing, File Management, Claude, GPT, Image Generation
