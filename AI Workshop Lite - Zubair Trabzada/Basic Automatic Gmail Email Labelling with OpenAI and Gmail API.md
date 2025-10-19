# Workflow Analysis for Automatic Gmail Email Labelling with AI

## Description
This workflow automates the process of labeling emails in Gmail using OpenAI to categorize email content. It helps in organizing your inbox efficiently by automatically assigning relevant labels to incoming emails.

## Input Details
This workflow is triggered when a new email is received in Gmail.

## Process Summary
The workflow starts by retrieving new emails from Gmail. It then uses OpenAI to generate appropriate labels for the email based on its content. A custom function node processes the labels, and finally, the Gmail API is used to apply these generated labels to the corresponding emails.

## Output Details
The workflow assigns AI-generated labels to emails in Gmail. It updates the email with the given labels.
