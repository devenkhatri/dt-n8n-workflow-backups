# Workflow Analysis for Telegram AI Agent

## Description
This workflow creates an AI assistant accessible via Telegram, allowing users to interact with a large language model.

## Input Details
The workflow is triggered by new messages received in a Telegram chat.

## Process Summary
The workflow starts by listening for new messages in Telegram. It then retrieves recent chat history and sends it along with the new message to a large language model (LLM) for processing. The LLM generates a response, potentially incorporating content from a website if requested. Finally, the generated response is sent back to the user via Telegram.

## Output Details
The workflow sends AI-generated text responses back to the Telegram chat where the original message was received.
