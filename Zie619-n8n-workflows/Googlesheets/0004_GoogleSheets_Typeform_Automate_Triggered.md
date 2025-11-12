# Workflow Analysis for Typeform Feedback Workflow

## Description
This workflow automatically captures course feedback submitted via Typeform, evaluates whether the feedback is positive or negative based on a usefulness rating, and logs the results into separate Google Sheets for positive and negative feedback.

## Input Details
The workflow is triggered by new form submissions from a Typeform form, receiving data such as course usefulness rating and written opinion.

## Process Summary
When a new Typeform response is received, the workflow extracts the usefulness rating and written opinion. It then checks if the usefulness rating is 3 or higher. If so, the feedback is appended to a 'positive_feedback' Google Sheet; otherwise, it is added to a 'negative_feedback' sheet. The workflow includes error handling to manage any failures during execution.

## Output Details
The workflow outputs categorized feedback entries into two separate Google Sheets—one for positive feedback and one for negative feedback.

## Tags
typeform, google sheets, feedback, automation, data routing, error handling, n8n
