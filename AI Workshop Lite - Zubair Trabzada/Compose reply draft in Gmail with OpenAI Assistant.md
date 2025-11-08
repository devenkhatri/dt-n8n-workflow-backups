# Workflow Analysis for AI Assistant Email Reply Draft Generator

## Description
This workflow automatically processes incoming email messages tagged with specific labels, sends their content to an OpenAI Assistant to generate a reply, and then creates a draft of this AI-generated reply within the original Gmail thread. Once the draft is created, the trigger label is removed from the email thread.

## Input Details
The workflow is triggered every minute by a scheduler and retrieves email threads from Gmail that have specific labels.

## Process Summary
The workflow starts by fetching Gmail threads with designated labels. For each identified thread, it extracts the content of the last message and sends it to a pre-configured OpenAI Assistant to generate a reply. The AI-generated response, initially in Markdown, is converted to HTML and then formatted into a raw email message. This raw message is encoded into base64 before being added as a new draft to the original email thread in Gmail. Finally, the specific label that triggered the process is removed from the thread.

## Output Details
The workflow creates an email draft containing the AI-generated reply within the original Gmail thread and removes the processing label from that thread.
