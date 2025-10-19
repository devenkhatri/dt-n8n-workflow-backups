# Workflow Analysis for Angie, Personal AI Assistant with Telegram Voice and Text

## Description
This workflow creates a personal AI assistant named Angie that interacts with users via Telegram using both voice and text messages.

## Input Details
The workflow is triggered by an HTTP request received from Telegram, containing user messages (text or voice).

## Process Summary
The workflow first detects if the incoming Telegram message is a voice message or a text message. If it's a voice message, it transcribes the audio to text using a speech-to-text API. Then, it sends the transcribed text or the original text message to a large language model (LLM) to generate a response from Angie. Finally, it converts Angie's text response into speech if the original input was a voice message and sends the appropriate response (text or audio) back to the user via Telegram.

## Output Details
The workflow sends either a text message or an audio file (Angie's spoken response) back to the user via Telegram.
