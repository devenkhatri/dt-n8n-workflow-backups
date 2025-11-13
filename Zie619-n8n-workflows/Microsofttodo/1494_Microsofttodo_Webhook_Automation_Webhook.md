# Workflow Analysis for MiniBear Webhook

## Description
This workflow automates responses and actions based on messages received from a Line webhook. It intelligently processes various message types, including text and images, to streamline communication and data management.

## Input Details
This workflow is triggered by an incoming POST request to a Line webhook at the "minibear" path, receiving event data from Line users.

## Process Summary
The workflow starts by receiving a Line message via a webhook and immediately sends a loading animation back to the user. It then uses a switch to route messages based on their type: text messages starting with "T " create a task in Microsoft To Do, while other text messages are saved to Microsoft Teams. If an image is received, it downloads and uploads the image to Microsoft OneDrive, then uses AI to classify it as a namecard, text, or other image. For namecards, it extracts detailed contact information, creates a follow-up task in Microsoft To Do, sends the extracted data back to Line, and triggers another workflow for Excel integration. For other images, it extracts text or describes the image content, posts this to Microsoft Teams, and replies to Line. Unsupported message types receive a "not supported" reply.

## Output Details
The workflow sends various text replies and confirmations back to the Line user, creates tasks in Microsoft To Do, saves messages and image analysis to Microsoft Teams, uploads images to Microsoft OneDrive, and triggers another workflow for Microsoft Excel integration.

## Tags
Line, Webhook, Microsoft Teams, Microsoft To Do, Microsoft OneDrive, AI, Image Processing, Text Extraction, Namecard, Automation
