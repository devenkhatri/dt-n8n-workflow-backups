# Workflow Analysis for Lead Capture and Notification Workflow

## Description
This workflow captures lead information via a web form, validates the email address, and then logs the lead in Google Sheets while simultaneously sending notifications via Gmail and Discord.

## Input Details
The workflow is triggered by form submissions containing Name, Email, and a Query message.

## Process Summary
The workflow starts when a user submits a form with their name, email, and query. It then verifies the email address using the Hunter email validation service. If the email is valid, the workflow proceeds to log the lead details—including submission timestamp—into a Google Sheet. Simultaneously, it sends an email notification to a specified Gmail address and posts a rich embed message to a Discord channel. If the email fails validation, the workflow stops and does not proceed with notifications or logging.

## Output Details
The workflow outputs lead data to a Google Sheet and sends notifications via Gmail and Discord with the lead details.

## Tags
lead capture, form automation, email validation, Google Sheets, Gmail, Discord, n8n, production-ready
