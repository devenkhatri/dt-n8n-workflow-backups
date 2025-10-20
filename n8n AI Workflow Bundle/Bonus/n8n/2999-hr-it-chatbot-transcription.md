# Workflow Analysis for HR/IT Chatbot Audio Transcription and Summary

## Description
This workflow transcribes audio inputs from an HR/IT chatbot, generates a summary, and logs the interaction.

## Input Details
This workflow is triggered manually and receives an audio file URL as input.

## Process Summary
The workflow starts by retrieving an audio recording URL from the input. It then downloads the audio file from the provided URL. Next, the downloaded audio file is transcribed into text using OpenAI's Whisper model. Following transcription, the text is summarized into a concise interaction summary using OpenAI's GPT-3.5 model. Finally, the chatbot ID, transcribed text, and interaction summary are compiled into a JSON object.

## Output Details
The workflow outputs a JSON object containing the chatbot ID, the full transcription, and a summary of the interaction.
