# Workflow Analysis for Detect toxic language in Telegram messages

## Description
This workflow monitors Telegram messages and automatically responds with a warning if a message contains toxic language such as profanity, identity attacks, or threats.

## Input Details
The workflow is triggered by incoming Telegram messages, including edits and channel posts, and receives the message text and metadata via a Telegram webhook.

## Process Summary
When a message is received from Telegram, the workflow sends the message text to Google Perspective API to analyze it for toxicity, specifically checking for profanity, identity attacks, and threats. It then evaluates whether the profanity score exceeds a threshold of 0.7. If the threshold is exceeded, the workflow sends an automated warning message back to the Telegram chat, replying directly to the offending message. If the message is not toxic enough, the workflow ends without action.

## Output Details
If toxic language is detected, the workflow sends a warning message via Telegram to the same chat where the original message was posted, replying directly to the offending message.

## Tags
telegram, moderation, toxicity detection, google perspective, profanity filter
