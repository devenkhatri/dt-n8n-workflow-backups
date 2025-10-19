# Workflow Analysis for n8n Workflow Generator

## Description
This workflow uses an AI model (OpenAI) to automatically generate complete n8n workflow code based on a user's textual request. After generation, it prepares the content, saves it as a local file, uploads this newly created workflow file to a designated folder in Google Drive, and sends a notification to a Discord channel to alert stakeholders of the new workflow creation.

## Input Details
The workflow is triggered manually (Start node) and requires the user to input a prompt describing the desired n8n workflow they want the AI to generate.

## Process Summary
The workflow begins by collecting a text prompt from the user describing the desired automation. This prompt is then sent to the OpenAI Chat API, which is configured to act as an n8n workflow generating AI. The AI's JSON response is received, and a unique filename is dynamically created based on the user's initial request. The generated content is then written to a file locally, which is subsequently uploaded to a specified folder within Google Drive. Finally, a message confirming the successful creation and upload of the new workflow is sent to a Discord channel.

## Output Details
The workflow produces a new n8n workflow file (JSON) which is saved locally, uploaded to Google Drive for secure storage, and an automated notification is sent to a Discord channel confirming the action.
