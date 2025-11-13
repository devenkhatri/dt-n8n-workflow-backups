# Workflow Analysis for Mattermost Workflow

## Description
This workflow processes customer feedback submitted via Typeform, analyzes its sentiment using AWS Comprehend, and notifies a Mattermost channel if the feedback is identified as negative.

## Input Details
The workflow is triggered by new submissions to a specified Typeform form and receives the submitted form data.

## Process Summary
First, the workflow is initiated when a new submission is received from Typeform. Next, the text from the form submission is sent to AWS Comprehend to determine its sentiment. An "If" node then evaluates whether the detected sentiment is negative. If the sentiment is negative, a message containing the feedback and its negative sentiment score is posted to a designated Mattermost channel. If the sentiment is not negative, the workflow proceeds to a "NoOp" node, completing its execution without further action on that path.

## Output Details
The workflow sends an informational message to a Mattermost channel when negative feedback is detected.

## Tags
automation, n8n, production-ready, excellent, optimized
