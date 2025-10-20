# Workflow Analysis for Telegram Speech Assistant

## Description
This workflow acts as an AI speech assistant via Telegram, transcribing voice messages, processing them with an AI model, and responding with text-to-speech.

## Input Details
The workflow is triggered by an incoming voice message to a Telegram bot.

## Process Summary
First, the workflow receives a voice message from Telegram and extracts the audio file. Next, it transcribes the audio into text using OpenAI Whisper. This transcribed text is then sent to an AI chat model (like ChatGPT) to generate a response. Finally, the AI-generated text response is converted back into speech using a text-to-speech API (like Eleven Labs) and sent back to the user via Telegram.

## Output Details
The workflow sends an AI-generated audio response back to the user via Telegram.
