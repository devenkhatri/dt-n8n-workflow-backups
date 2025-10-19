# Workflow Analysis for Extract Personal Data with Self-Hosted LLM

## Description
This workflow extracts personal information like name, email, phone number, and address from a given text using a self-hosted Mistral LLM via the NeMo Integrations API and stores the extracted data in a Google Sheet.

## Input Details
The workflow is triggered manually and takes a text input containing personal data.

## Process Summary
The workflow starts by receiving text input. It then prepares a prompt for the Mistral LLM to extract specific personal data fields. It sends this prompt to the NeMo Integrations API, which uses a self-hosted Mistral model to process the text. Finally, it takes the extracted personal data and appends it as a new row in a specified Google Sheet.

## Output Details
The workflow appends the extracted personal data (Name, Email, Phone, Address) as a new row in a Google Sheet.
