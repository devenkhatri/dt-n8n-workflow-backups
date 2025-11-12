# Workflow Analysis for Emelia Workflow

## Description
This workflow automates the creation of an email marketing campaign in Emelia and adds a contact to it. It is designed for production use with error handling and reliable execution.

## Input Details
The workflow is triggered manually and does not receive external input data.

## Process Summary
The workflow starts with a manual trigger. It then creates a new campaign named 'n8n-docs' in Emelia. Next, it attempts to add a contact with a placeholder email and name to a hardcoded campaign ID. A third Emelia node references the newly created campaign ID from the first step (though it doesn't perform a specified operation). If any step fails, the workflow routes to an error handler that stops execution and displays an error message.

## Output Details
The workflow creates a campaign and adds a contact in Emelia; it does not return data externally but may log execution results within n8n.

## Tags
emelia, email marketing, automation, manual trigger, campaign creation, contact management, n8n
