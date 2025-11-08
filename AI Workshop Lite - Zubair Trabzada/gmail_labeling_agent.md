# Workflow Analysis for AI-Powered Gmail Email Labeler

## Description
This workflow uses artificial intelligence to automatically categorize and label incoming emails in Gmail, streamlining inbox management and improving organization for users.

## Input Details
The workflow is triggered every minute by new emails in a specified Gmail account, receiving the email's content and metadata.

## Process Summary
The workflow initiates by checking for new emails in a designated Gmail account. It then extracts the text content of each new email and sends it to an AI agent for classification. The AI agent, utilizing an OpenAI chat model, categorizes the email into one of four predefined labels: Sponsorship, Collaboration, Business Inquiries, or Others. Finally, based on the AI's classification, the workflow applies the corresponding label to the original email within Gmail.

## Output Details
The workflow assigns one of four predefined labels (Sponsorship, Collaboration, Business Inquiries, or Others) to incoming Gmail emails.
