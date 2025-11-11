# Workflow Analysis for Reply draft with OpenAI Assistant

## Description
This workflow automatically monitors incoming Gmail messages with specific labels, sends the latest message content to an OpenAI Assistant for a response, creates an HTML-formatted reply draft in the same email thread, and removes the trigger label once the draft is created.

## Input Details
The workflow is triggered every minute by a schedule to check for Gmail threads labeled with a specific trigger label.

## Process Summary
The workflow first retrieves Gmail threads with a specific label. For each thread, it fetches all messages, isolates the latest message, and extracts its content. This content is sent to a predefined OpenAI Assistant, which generates a reply. The assistant’s markdown response is converted to HTML, wrapped into a properly formatted raw email message, encoded in base64, and added as a draft reply to the original thread. Finally, the trigger label is removed from the thread.

## Output Details
The workflow creates a reply draft in the original Gmail thread using the AI-generated response and removes the trigger label from that thread.

## Tags
Gmail, OpenAI Assistant, Email Automation, AI Reply, Draft Email, Scheduled Workflow
