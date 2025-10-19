# Workflow Analysis for Telegram Toxic Language Detector

## Description
This workflow monitors a specified Telegram chat for new messages, identifies if a message contains toxic language using a toxicity detection API, and replies to the sender if toxicity is detected.

## Input Details
The workflow is triggered by new messages in a Telegram chat.

## Process Summary
The workflow receives new messages from a Telegram chat. It then calls an external API to check if the message content contains toxic language. If toxicity is detected, the workflow branches to send a reply message back to the sender in the Telegram chat, informing them about the toxic content. Otherwise, it ends without further action.

## Output Details
The workflow sends a reply message in Telegram if toxic language is detected.
