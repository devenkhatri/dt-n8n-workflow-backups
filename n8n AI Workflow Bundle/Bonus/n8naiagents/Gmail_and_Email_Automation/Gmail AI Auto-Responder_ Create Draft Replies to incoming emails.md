# Workflow Analysis for Gmail AI Auto-responder: Create Draft Replies to Incoming Emails

## Description
This workflow uses AI to automatically assess incoming Gmail emails and, if a reply is needed, generates a draft response in your Gmail account, allowing for quick review and sending.

## Input Details
This workflow is triggered every minute by new incoming emails in Gmail, excluding emails sent by the user.

## Process Summary
First, upon receiving a new email, an AI model assesses whether the email requires a reply. The output of this assessment, a boolean indicating if a reply is needed, is then parsed. If the AI determines a reply is necessary, another AI model is invoked to generate a draft email reply. This AI adheres to specific instructions for tone, structure, and content, including providing two options for yes/no questions. Finally, the generated reply is used to create a new draft email in Gmail, addressed to the original sender and linked to the existing conversation.

## Output Details
The workflow produces a draft email reply within the user's Gmail account, linked to the original email thread.
