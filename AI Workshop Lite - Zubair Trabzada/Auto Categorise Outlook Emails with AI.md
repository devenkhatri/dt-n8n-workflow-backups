# Workflow Analysis for Automated Outlook Email Categorization with AI

## Description
This workflow automatically categorizes incoming Outlook emails using AI, assigns appropriate categories, and moves them to designated folders to streamline email management.

## Input Details
The workflow is triggered manually and retrieves unread emails from a specified Outlook mail folder.

## Process Summary
First, the workflow fetches all unread emails from a designated Outlook folder. Each email's subject and body are then sent to a large language model (LLM) to determine a category. After categorizing, the workflow marks the processed emails as read. Finally, it uses the categorized output to move the email to the corresponding folder in Outlook.

## Output Details
The workflow categorizes and moves Outlook emails to specific folders and sends success/failure notifications to a specified email address.
