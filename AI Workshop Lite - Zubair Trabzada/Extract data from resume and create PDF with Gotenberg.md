# Workflow Analysis for Telegram Resume Extractor

## Description
This workflow automates the extraction of resume data from a PDF document uploaded via Telegram, structures it using AI, formats it into a readable HTML, and then converts it into a new PDF document which is sent back to the user.

## Input Details
The workflow is triggered by a document upload (specifically a PDF resume) to a configured Telegram bot.

## Process Summary
The workflow initiates upon a PDF resume upload to a Telegram bot, first performing an authentication check and ignoring /start messages. It downloads the PDF, extracts its text content, and then uses an OpenAI GPT-4 model with an auto-fixing and structured output parser to transform the raw text into a comprehensive JSON object of resume data. Subsequently, various code nodes convert different sections of this structured JSON (e.g., employment history, education, projects) into HTML format. These HTML components are then merged, encoded to base64, converted into an HTML file, and finally sent to a Gotenberg server to generate a new, formatted PDF document.

## Output Details
The workflow delivers a newly generated PDF file, containing the structured and formatted resume information, back to the user via Telegram.
