# Workflow Analysis for Telegram Profanity Checker and Responder

## Description
This workflow monitors incoming Telegram messages, analyzes them for profanity using Google Perspective, and automatically responds to the sender if the message is deemed toxic.

## Input Details
The workflow is triggered by new or edited messages and channel posts received from a configured Telegram bot.

## Process Summary
1. The workflow starts when a message is received via Telegram.
2. The text content of the message is then sent to Google Perspective API for sentiment analysis, specifically checking for identity attacks, threats, and profanity.
3. An 'If' node evaluates the profanity score returned by Google Perspective.
4. If the profanity score is above 0.7, a "I don't tolerate toxic language!" message is sent as a reply to the original message in Telegram.
5. If the profanity score is not above 0.7, no further action is taken by this branch.

## Output Details
The workflow sends a warning message back to the Telegram chat as a reply if profanity is detected in the incoming message.

## Tags
telegram, profanity detection, content moderation, google perspective, automation, messaging, conditional logic, error handling, n8n, production-ready, excellent, optimized
