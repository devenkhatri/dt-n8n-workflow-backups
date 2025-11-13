# Workflow Analysis for Mattermost Workflow

## Description
This workflow automatically processes feedback submitted via Typeform, analyzes its sentiment, and notifies a Mattermost channel if the feedback is negative.

## Input Details
The workflow is triggered by new submissions to a specific Typeform, receiving form data including user feedback.

## Process Summary
1. The workflow starts when a new form is submitted via Typeform. 2. It then sends the submitted feedback text to AWS Comprehend to detect the sentiment (e.g., positive, negative, neutral). 3. An If node checks if the detected sentiment is negative. 4. If the sentiment is negative, a message containing the feedback and its negative score is sent to a specific Mattermost channel. 5. If the sentiment is not negative, the workflow proceeds to a NoOp node, which effectively does nothing further.

## Output Details
The workflow sends a notification to a Mattermost channel with details of negative feedback, or it completes without further action if the feedback is not negative.

## Tags
automation, feedback, sentiment analysis, Mattermost, Typeform, AWS Comprehend
