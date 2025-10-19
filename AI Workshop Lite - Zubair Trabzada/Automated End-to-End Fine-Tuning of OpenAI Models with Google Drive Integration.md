# Workflow Analysis for Automated OpenAI Fine-Tuning with Google Drive

## Description
This workflow automates the end-to-end process of fine-tuning OpenAI models using data from Google Drive, handling file preparation, model training, and notification.

## Input Details
The workflow is triggered manually.

## Process Summary
The workflow starts by creating a new folder in Google Drive for processed files. It then reads a CSV file from a specified Google Drive folder, combines and cleans the data, and converts it into a JSONL format suitable for OpenAI fine-tuning. This prepared file is uploaded to OpenAI, a fine-tuned model is created, and the workflow waits for its completion. Finally, it sends a Discord notification with the fine-tuning job details.

## Output Details
The workflow creates a fine-tuned OpenAI model and sends a Discord notification with the job details.
