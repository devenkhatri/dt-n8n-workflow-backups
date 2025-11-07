# Workflow Analysis for AI Email Agent

## Description
This AI agent workflow is designed to help users send emails by processing their chat queries. It identifies email recipients, subjects, and bodies, and can retrieve missing contact information from a database before sending the email.

## Input Details
The workflow is triggered by a chat message and receives user queries as input.

## Process Summary
The workflow is initiated upon receiving a chat message. An AI agent then analyzes the chat message to determine if an email needs to be sent, identifying the recipient, subject, and body. If the recipient's email address is not provided, the AI agent queries a Google Sheets-based contact database to retrieve it. Once all necessary email details are collected, the agent composes and sends the email using a Gmail tool. Finally, the AI agent provides a confirmation of the email sending status back to the user.

## Output Details
The workflow sends emails via Gmail and returns the AI agent's response, confirming the email status, to the chat.
