# Workflow Analysis for Telegram AI Assistant

## Description
This workflow creates an AI Assistant accessible via Telegram, enabling users to interact with a Large Language Model (LLM) for various queries and tasks directly within their Telegram chat.

## Input Details
The workflow is triggered by an incoming message to a configured Telegram bot, which provides the user's query and chat ID.

## Process Summary
The workflow starts by extracting the user's message and chat ID from the Telegram update. It then constructs a comprehensive prompt for the LLM, including system instructions and the user's query. The prompt is sent to the LLM (e.g., OpenAI's GPT) for processing. The LLM's response is then extracted, cleaned, and formatted. Finally, the processed response is sent back to the user via Telegram.

## Output Details
The workflow responds to the user's Telegram message with the generated AI-powered answer.
