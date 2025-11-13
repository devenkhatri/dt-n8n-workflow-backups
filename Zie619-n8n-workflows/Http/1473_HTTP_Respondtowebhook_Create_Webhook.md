# Workflow Analysis for Generate Text-to-Speech Using Elevenlabs via API

## Description
This workflow provides an API endpoint to convert text into speech using Elevenlabs.io. It requires custom authentication with an Elevenlabs API key.

## Input Details
The workflow is triggered by a POST request to the "/generate-voice" webhook, expecting `voice_id` and `text` as parameters in the request body.

## Process Summary
First, the workflow receives a POST request via a webhook. It then validates if both `voice_id` and `text` are present in the request. If the required parameters exist, it makes an HTTP POST request to the Elevenlabs API to generate speech, using the provided text and custom authentication. Finally, the generated audio is returned to the original webhook. If the initial parameters are invalid, an error message is returned.

## Output Details
The workflow either returns the generated speech as binary data or a JSON error message if the input parameters are invalid.

## Tags
automation, n8n, production-ready, text-to-speech, Elevenlabs, API
