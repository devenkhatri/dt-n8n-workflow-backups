# Workflow Analysis for Fetch and Process Typeform Submissions

## Description
This workflow processes new submissions from a Typeform form, extracts specific answers, and then relays this information to a custom webhook.

## Input Details
The workflow is triggered by new submissions to a specified Typeform form via a webhook.

## Process Summary
The workflow starts by waiting for a new Typeform submission. It then extracts the value of a specific answer ("Name" in this case) from the form submission data. Next, it combines the extracted answer with a predefined message. Finally, it sends this combined data as a POST request to a custom webhook URL.

## Output Details
The workflow sends a POST request to a custom webhook with the processed data, including the extracted Typeform answer.
