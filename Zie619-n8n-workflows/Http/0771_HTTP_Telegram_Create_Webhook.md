# Workflow Analysis for Telegramtrigger Workflow

## Description
This workflow automatically processes incoming Telegram messages—either voice or text—and generates social media content along with a detailed image prompt based on the user's request. Voice messages are transcribed into text using OpenAI's Whisper API before being processed further.

## Input Details
The workflow is triggered by incoming Telegram messages, which can be either text or voice messages from users.

## Process Summary
The workflow starts by receiving Telegram messages. It checks whether the message contains voice or text. If it's a voice message, it fetches the audio file from Telegram and transcribes it into text using OpenAI. The resulting or original text is then passed to an AI agent that uses SerpAPI to research the topic, generates SEO-optimized social media content, and creates a detailed image prompt. Finally, the image prompt is sent to an external service to generate an actual image.

## Output Details
The workflow outputs generated social media content and an image created from the AI-generated prompt, which can be sent back to the user or used elsewhere.

## Tags
Telegram, AI Agent, OpenAI, SerpAPI, Voice Transcription, Social Media Content, Image Generation, Automation, n8n
