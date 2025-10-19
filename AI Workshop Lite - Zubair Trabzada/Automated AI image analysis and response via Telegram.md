# Workflow Analysis for Automated AI Image Analysis and Telegram Response

## Description
This workflow automates the process of receiving image inputs via Telegram, analyzing them using an AI model, and sending the analysis results back to the user on Telegram.

## Input Details
The workflow is triggered by an incoming message to a Telegram bot.

## Process Summary
The workflow starts by consuming the Telegram message. It then checks if an image is present in the message. If an image is found, it downloads the image. The image is then sent to an AI model for analysis. Finally, the analysis result is formatted and sent back as a message to the user on Telegram by Telegram bot.

## Output Details
The workflow sends the AI analysis results as a text message back to the user on Telegram.
