# Workflow Analysis for Nano Photoshop Agent

## Description
A Telegram-based AI assistant that helps users manage, edit, and generate images using AI. It can upload photos to Google Drive, rename them, combine images, search stored files, and edit images based on user requests.

## Input Details
The workflow is triggered by messages sent to a Telegram bot, which can include either text commands or photo uploads.

## Process Summary
The workflow starts by receiving a message from Telegram and uses a switch node to determine if the message contains a photo or text. If a photo is received, it downloads the image, uploads it to a Google Drive folder, and prepares a response with the file ID. If text is received (or after photo processing), it forwards the input to an AI agent powered by either GPT-5 Mini or Claude Sonnet 3.5. The AI agent uses tools to perform actions like renaming files, combining images, editing images, or searching Google Drive for existing files based on the user's request, then sends a response back via Telegram.

## Output Details
The workflow sends a response message back to the user in Telegram, which may include file links, confirmations of actions taken, or results from AI image operations.

## Tags
telegram, google drive, image editing, AI agent, file management, Claude, GPT, image generation
