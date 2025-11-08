# Workflow Analysis for AI Personal Assistant Workflow (Telegram Integrated)

## Description
This workflow enables users to interact with an AI personal assistant via Telegram. The assistant can process both text and voice messages to provide information from Google Calendar, unread Gmail emails, and manage tasks and contacts stored in Baserow.

## Input Details
The workflow is triggered by incoming messages (text or voice) received by a configured Telegram bot.

## Process Summary
The workflow listens for incoming Telegram messages, automatically determining if the input is text or a voice message. If it's a voice message, the audio is retrieved and transcribed into text using OpenAI. The processed text is then sent to an AI assistant, "Angie," which uses an OpenAI chat model and conversation memory. Angie can access and process information from Google Calendar, unread Gmail emails, and manage data in Baserow for tasks and contacts. Finally, the AI assistant's response is sent back to the user via Telegram.

## Output Details
The workflow sends a structured text response from the AI assistant back to the user on Telegram.
