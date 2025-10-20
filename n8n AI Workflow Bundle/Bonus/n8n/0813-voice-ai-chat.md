# Workflow Analysis for Voice AI Chatbot

## Description
This workflow enables a voice-activated AI chatbot experience by transcribing audio input, processing it with an AI model, and converting the AI's response back to speech.

## Input Details
The workflow is triggered by an HTTP request containing an audio file.

## Process Summary
The workflow receives an audio file, transcribes the audio to text using a speech-to-text API, and sends this text to an AI model for a conversational response. The AI's text response is then converted into an audio file using a text-to-speech API. Finally, the workflow clears the chat history and returns the generated audio.

## Output Details
The workflow returns an audio file containing the AI chatbot's spoken response.
