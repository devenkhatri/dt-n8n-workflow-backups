# Workflow Analysis for Retell Inbound Call Dynamic Variables Handler

## Description
This workflow integrates with Retell AI to dynamically fetch user data from a Google Sheet based on the caller's phone number and return it as dynamic variables for use in Retell voice agent prompts.

## Input Details
The workflow is triggered by a POST webhook from Retell AI containing the inbound call's phone number, and it receives this data from Retell's servers (restricted to a specific IP address).

## Process Summary
The workflow starts by receiving a webhook from Retell AI during an inbound call. It extracts the caller's phone number from the request payload. It then queries a Google Sheet to find a matching user record using the phone number. Once found, it maps specific fields from the sheet (like first name, last name, email, and custom variables) into a structured JSON response. Finally, it sends this JSON back to Retell to populate dynamic variables in the agent's conversation flow.

## Output Details
The workflow returns a JSON response to Retell AI containing dynamic user variables that are used to personalize the voice agent's conversation during the call.

## Tags
Retell AI, voice agent, dynamic variables, Google Sheets, inbound call, webhook, n8n, automation, customer data, personalization
