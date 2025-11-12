# Workflow Analysis for n8n Graphic Design Team

## Description
This workflow automates the generation, review, and storage of AI-generated images based on user-submitted creative briefs. It uses Ideogram to create images from prompts, stores them in Google Drive, logs metadata in Google Sheets, and optionally uses AI to evaluate and refine images before final delivery.

## Input Details
The workflow is triggered by a form submission containing an image prompt, target audience description, and generation settings like aspect ratio, model version, and style preferences.

## Process Summary
The workflow begins by capturing a creative brief via a form. It uses this input to generate an image with the Ideogram API, then downloads and uploads the image to a designated Google Drive folder. Image metadata is logged in a Google Sheet. Separately, an AI reviewer (using OpenAI) evaluates the image against audience and quality criteria, and if needed, triggers a remix with an improved prompt. Both original and remixed images are tracked in Sheets and Drive. A one-time setup flow also creates necessary folders and a tracking spreadsheet.

## Output Details
The workflow saves generated images to Google Drive, logs image metadata in Google Sheets, and optionally sends email notifications with links and setup instructions.

## Tags
AI image generation, Ideogram, Google Drive, Google Sheets, OpenAI review, automated design, graphic design automation, n8n workflow
