# Workflow Analysis for Telegram Profanity Detector

## Description
This workflow monitors incoming messages in a Telegram chat. If a message is identified as containing profanity by the Google Perspective API, the workflow automatically sends a reply indicating that toxic language is not tolerated.

## Input Details
The workflow is triggered by new or edited messages and channel posts received from a configured Telegram bot.

## Process Summary
First, the workflow receives a message from Telegram. Next, it sends the message's text to the Google Perspective API to analyze its profanity, identity attack, and threat scores. Then, it checks if the profanity score is greater than 0.7. If the score indicates high profanity, a predefined message is sent back to the original Telegram chat, replying to the profane message. Otherwise, the workflow proceeds without any action.

## Output Details
The workflow sends a "I don't tolerate toxic language!" message back to the Telegram chat if profanity is detected in the incoming message.
