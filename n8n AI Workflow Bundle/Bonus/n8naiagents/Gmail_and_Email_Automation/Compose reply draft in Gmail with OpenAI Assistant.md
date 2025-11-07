# Workflow Analysis for Automated Gmail Reply Drafts using OpenAI Assistant

## Description
This workflow automates the process of generating email reply drafts. It monitors your Gmail account for incoming emails with specific trigger labels, forwards the email content to an OpenAI Assistant for a response, and then creates a draft reply in the original email thread. Once the draft is created, the trigger label is removed from the email.

## Input Details
The workflow is triggered every minute, scanning Gmail for threads that have specific predefined labels.

## Process Summary
1. The workflow initiates on a recurring 1-minute schedule.
2. It fetches all Gmail threads that have been assigned a designated trigger label.
3. For each identified thread, it retrieves the content of the latest message and sends it to a specified OpenAI Assistant.
4. The OpenAI Assistant processes the message and generates a reply, which is then converted from Markdown into HTML format.
5. Finally, this HTML reply is assembled into a raw email, encoded in base64, and added as a new draft to the original Gmail thread, after which the trigger label is removed from the thread.

## Output Details
The workflow generates an AI-powered reply draft within the corresponding Gmail thread and removes the specific trigger label used for processing.
