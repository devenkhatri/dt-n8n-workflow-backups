# Workflow Analysis for Generate Text-to-Speech Using ElevenLabs via API

## Description
This workflow provides an API endpoint that converts text into speech using ElevenLabs' text-to-speech service. It validates required input parameters and returns the generated audio or an error message if inputs are missing.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint with two required parameters: 'voice_id' and 'text'.

## Process Summary
The workflow starts with a webhook that receives a POST request containing 'voice_id' and 'text'. An 'If' node checks whether both parameters exist. If they do, the workflow sends a request to the ElevenLabs API to generate speech from the provided text using the specified voice. The resulting audio is returned as a binary response. If either parameter is missing, the workflow returns a JSON error message indicating invalid inputs.

## Output Details
The workflow returns either the generated audio file as a binary response or a JSON error message if the input parameters are missing.

## Tags
text-to-speech, ElevenLabs, API, webhook, audio generation, n8n, automation
