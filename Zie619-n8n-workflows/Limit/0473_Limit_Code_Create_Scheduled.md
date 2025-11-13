# Workflow Analysis for Reply draft with OpenAI Assistant

## Description
This workflow automatically transfers content of incoming email messages with specific labels into an OpenAI Assistant to generate a reply draft. After the draft is composed, the trigger label is deleted from the thread.

## Input Details
The workflow is triggered every minute and processes incoming email threads from Gmail that have specific labels.

## Process Summary
The workflow first fetches Gmail threads with a designated trigger label. For each thread, it retrieves the content of the latest message and sends it to an OpenAI Assistant to generate a reply. The AI's response is then converted to HTML, formatted into a raw email, and base64 encoded. Finally, this encoded email is added as a draft to the original Gmail thread, and the trigger label is removed.

## Output Details
The workflow creates and inserts an AI-generated email reply draft into the relevant Gmail thread and removes the processing label from that thread.

## Tags
Automation, n8n, Production-ready, Excellent, Optimized, Gmail, OpenAI, Email Automation, AI Assistant, Reply Draft
