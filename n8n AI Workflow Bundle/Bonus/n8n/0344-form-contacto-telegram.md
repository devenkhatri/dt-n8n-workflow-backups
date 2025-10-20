# Workflow Analysis for Contact Form to Telegram

## Description
This workflow captures form submissions from a webhook, extracts relevant contact information, and sends a formatted message to a specified Telegram chat.

## Input Details
The workflow is triggered by an HTTP webhook that receives form submission data.

## Process Summary
The workflow starts by receiving data from a webhook. It then extracts the name, email, and message from the received JSON data. The extracted information is used to construct a formatted text message. Finally, this message is sent to a specified Telegram chat.

## Output Details
The workflow sends a contact message to a Telegram chat.
