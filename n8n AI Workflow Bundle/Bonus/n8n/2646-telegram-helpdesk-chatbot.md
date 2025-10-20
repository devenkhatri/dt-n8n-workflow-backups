# Workflow Analysis for Telegram Helpdesk Chatbot

## Description
This workflow automates a helpdesk chatbot on Telegram. It processes incoming messages, generates AI responses, and stores conversation history.

## Input Details
The workflow is triggered by new messages received via a Telegram Bot.

## Process Summary
First, the workflow extracts information from the incoming Telegram message. Next, it retrieves the conversation history between the user and the bot from a Baserow database. Then, it sends the conversation history and the new message to an AI model to generate a response. Subsequently, the generated AI response is sent back to the user via Telegram. Finally, the new message and the AI's response are saved as new records in the Baserow database.

## Output Details
The workflow sends AI-generated responses back to the user on Telegram and updates a Baserow database with the conversation history.
