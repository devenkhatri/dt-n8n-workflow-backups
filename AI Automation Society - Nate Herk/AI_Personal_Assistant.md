# Workflow Analysis for AI Personal Assistant

## Description
An AI-powered personal assistant that interacts with users via Telegram, handles both text and voice messages, and can perform tasks such as managing contacts, sending emails, scheduling calendar events, retrieving project information, and conducting online research.

## Input Details
The workflow is triggered by incoming Telegram messages, which can be either text or voice messages from a user.

## Process Summary
The workflow first checks if the incoming Telegram message is text or voice. Voice messages are downloaded and transcribed into text using OpenAI's speech-to-text capability. The text (either original or transcribed) is then passed to an AI agent that uses a custom prompt defining its role as a personal assistant. The agent has access to several tools: a Google Sheets contact database, email and calendar agents (implemented as sub-workflows), a research agent for internet searches, and a Pinecone vector store for retrieving company project information. The agent's response is sent back to the user via Telegram as text and also converted into audio using ElevenLabs' text-to-speech API and sent as a voice message.

## Output Details
The workflow sends two responses back to the user on Telegram: a text message with the AI's answer and a voice message with the spoken version of the response.

## Tags
AI Agent, Telegram Bot, Voice Assistant, Personal Assistant, OpenAI, Google Sheets, Calendar Integration, Email Automation, Research Agent, Text-to-Speech, Voice-to-Text, Pinecone, Vector Store
