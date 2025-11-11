# Workflow Analysis for Automated Image Analysis and Response via Telegram

## Description
This workflow automatically analyzes images sent to a Telegram bot using OpenAI and sends back a detailed description of the image content. If no image is sent, it replies with an error message prompting the user to upload an image.

## Input Details
The workflow is triggered when a user sends a message to a Telegram bot, and it checks whether the message includes an image.

## Process Summary
The workflow starts by listening for messages via a Telegram bot trigger. It uses a Switch node to determine if the message contains an image. If an image is present, it sends the image (in base64 format) to OpenAI for analysis. The resulting description from OpenAI is then sent back to the user via Telegram. If no image is detected, the workflow waits briefly and sends an error message asking the user to upload an image.

## Output Details
The workflow sends either an AI-generated description of the image or an error message back to the Telegram chat where the original message was sent.

## Tags
Telegram, OpenAI, Image Analysis, Automation, AI, Bot, Messaging
