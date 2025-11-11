# Workflow Analysis for Resume Extractor and PDF Generator

## Description
This workflow automatically extracts structured data from a resume PDF sent via Telegram, converts it into a well-formatted HTML document, and returns a polished PDF version back to the user.

## Input Details
The workflow is triggered when a user sends a PDF resume file via Telegram to a configured bot.

## Process Summary
The workflow first authenticates the Telegram user and ignores '/start' messages. It downloads the uploaded PDF, extracts its text content, and uses OpenAI's GPT-4 Turbo model with a structured JSON schema to parse personal info, work history, education, projects, and other resume sections. Each parsed section is then converted into formatted HTML. All HTML sections are merged, converted to a base64-encoded HTML file, and transformed into a PDF using Gotenberg. Finally, the generated PDF is sent back to the user on Telegram.

## Output Details
The workflow produces a formatted PDF version of the resume and sends it back to the user via Telegram.

## Tags
resume parsing, PDF generation, Telegram bot, OpenAI, HTML conversion, structured data extraction, Gotenberg, automation
