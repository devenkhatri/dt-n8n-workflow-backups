# Workflow Analysis for AI Personal Assistant

## Description
This workflow acts as an AI personal assistant accessible via Telegram, capable of understanding both text and voice commands to manage various tasks.

## Input Details
This workflow is triggered by incoming messages from Telegram, which can be either text or voice.

## Process Summary
The workflow is triggered by incoming text or voice messages from Telegram. If a voice message is received, it is downloaded and transcribed into text using OpenAI. The text input is then processed by an OpenAI-powered personal assistant, which leverages a conversational memory and an array of specialized tools including a Google Sheets contact database, email and calendar agents, an internet research agent, and a vector store for project information. After the AI agent generates a response, it is summarized and then sent back to the user on Telegram, either as a text message or converted into an audio reply via Eleven Labs.

## Output Details
The workflow sends a response back to the Telegram chat, which can be either a text message or an audio message generated from the AI's reply.
