# Workflow Analysis for Email Header Analyzer

## Description
This workflow analyzes email headers to extract key information and determine the sender's legitimacy using an AI model. It helps in identifying potential spam or phishing attempts.

## Input Details
The workflow is triggered manually and requires the user to input raw email headers.

## Process Summary
The workflow starts by taking raw email headers as input. It then extracts specific data points like "Return-Path," "Reply-To," "From," "Subject," and "Received-SPF." These extracted fields are then combined into a single string. Finally, this combined string is sent to an AI model for analysis, and the AI's response is extracted.

## Output Details
The workflow outputs the AI model's analysis of the email headers, indicating the sender's legitimacy.
