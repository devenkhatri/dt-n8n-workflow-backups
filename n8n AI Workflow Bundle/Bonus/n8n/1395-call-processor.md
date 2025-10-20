# Workflow Analysis for Call Processor with AI Analysis and CRM Update

## Description
This workflow processes new voicemails and call recordings, transcribes them using AI, analyzes the content for key information, and then updates a CRM system with the extracted data.

## Input Details
This workflow is triggered when a new voicemail or call recording is received from an external platform via a webhook.

## Process Summary
The workflow starts by extracting the voicemail data, including the audio file. It then uses an AI model to transcribe the audio into text. Next, another AI model analyzes the transcribed text to identify key information like caller intent, sentiment, lead status, lead source, and product interest. The workflow then prepares this extracted information for insertion or update in a CRM system. Finally, it either creates a new record or updates an existing one in the CRM with the processed call data and AI analysis.

## Output Details
The workflow updates a CRM system with transcribed call content, AI-extracted insights, and other relevant call details.
