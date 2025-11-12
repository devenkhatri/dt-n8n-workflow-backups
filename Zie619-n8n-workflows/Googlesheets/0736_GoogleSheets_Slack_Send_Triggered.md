# Workflow Analysis for Typeformtrigger Workflow

## Description
This workflow automatically captures user-submitted problem reports from a Typeform, logs them into a Google Sheet, and sends high-severity issues (severity > 7) to both Slack and email for immediate attention.

## Input Details
The workflow is triggered by a form submission from a specific Typeform (Form ID: UXuY0A), receiving data such as the user's name, email, problem description, and severity rating.

## Process Summary
When a user submits a problem report via Typeform, the workflow appends the data to a Google Sheet named 'Problems'. It then checks if the severity score is greater than 7. If so, it sends a detailed alert message to a Slack channel named 'problems' and simultaneously emails the report to a designated recipient. The message includes the user's contact info, severity level, and problem description.

## Output Details
The workflow logs all submissions in a Google Sheet and, for high-severity issues, sends notifications via both Slack and email.

## Tags
Typeform, Google Sheets, Slack, Email, Alerting, Severity-based Routing, Automation, Support Ticketing
