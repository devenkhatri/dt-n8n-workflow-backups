# Workflow Analysis for Text Classifier

## Description
This workflow automatically labels incoming Gmail emails into predefined categories such as Sponsorship, Collaboration, Business Inquiries, or Others using an AI classification model.

## Input Details
The workflow is triggered by new emails received in a Gmail inbox and processes the email text content.

## Process Summary
The workflow starts by monitoring the Gmail inbox for new emails. When an email arrives, its text is sent to an AI-powered text classifier that uses the GPT-4o-mini model to categorize the email into one of four predefined labels. Based on the AI's classification, the workflow adds the appropriate Gmail label to the email. Each possible label (Sponsorship, Collaboration, Business Inquiries, Others) has a dedicated Gmail node to apply the corresponding label. The system runs automatically on a schedule (every minute) to check for new emails.

## Output Details
The workflow labels incoming Gmail messages with the appropriate category label based on AI classification.

## Tags
gmail, ai, email classification, labeling, automation, openai, text classifier
