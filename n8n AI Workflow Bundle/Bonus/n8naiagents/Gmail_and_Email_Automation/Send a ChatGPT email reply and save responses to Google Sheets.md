# Workflow Analysis for Automated ChatGPT Email Reply and Google Sheets Logging with Feedback

## Description
This workflow automates email responses using OpenAI's ChatGPT and records the interaction in Google Sheets. It listens for incoming emails, generates a reply, and sends it back to the sender. It also includes a feedback mechanism in the sent email, allowing recipients to rate the AI's response, which is then recorded in the same Google Sheet for potential fine-tuning.

## Input Details
The workflow is triggered either by receiving a new email through Gmail, providing email content (sender, recipient, subject, body), or by a webhook when a feedback link (containing an ID and feedback like "Yes" or "No") in a previously sent email is clicked.

## Process Summary
1. Upon receiving an email from a specified recipient, the workflow extracts the message content and checks if it's within the token limit. 2. If the message is suitable, it uses OpenAI to generate an automated reply. 3. The generated reply is then formatted into an HTML email, including a unique ID and feedback links (Yes/No), and sent back to the original sender via Gmail. 4. Concurrently, the initial email content, the generated reply, and a unique ID are stored in a Google Sheet. If the specified spreadsheet or worksheet does not exist, it is created automatically. 5. If a feedback link in the sent email is clicked, a separate webhook trigger updates the corresponding entry in the Google Sheet with the 'Yes' or 'No' feedback, and a "Thanks for your response!" HTML page is displayed.

## Output Details
The workflow sends automated HTML email replies with feedback links to the original senders and stores conversation data (initial message, generated reply, and user feedback) in a Google Sheet.
