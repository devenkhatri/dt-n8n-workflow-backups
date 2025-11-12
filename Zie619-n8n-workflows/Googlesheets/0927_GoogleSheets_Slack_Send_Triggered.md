# Workflow Analysis for Typeformtrigger Workflow

## Description
This workflow automatically captures user-submitted problem reports from a Typeform, logs them in a Google Sheet, and—when the reported issue severity is greater than 7—sends alerts via both email and Slack to notify the team.

## Input Details
The workflow is triggered by a form submission from a Typeform with form ID 'UXuY0A', receiving data such as the user's name, email, problem description, and severity rating.

## Process Summary
When a Typeform is submitted, the data is first appended to a Google Sheet in the 'Problems' tab. Then, an If node checks whether the 'Severity' value is greater than 7. If true, the workflow sends a detailed notification email and posts the same information to a Slack channel named 'problems'.

## Output Details
The workflow logs all submissions in Google Sheets and, for high-severity issues (severity > 7), sends an email and posts a message to Slack.

## Tags
Typeform, Google Sheets, Slack, Email Notification, Conditional Logic, Severity Alert, Automation, n8n
