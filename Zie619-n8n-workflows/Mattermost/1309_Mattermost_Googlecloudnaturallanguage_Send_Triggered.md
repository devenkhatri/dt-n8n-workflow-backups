# Workflow Analysis for Analyze the sentiment of feedback and send a message on Mattermost

## Description
Automated workflow: Analyze the sentiment of feedback and send a message on Mattermost. This workflow processes data and performs automated tasks.

## Input Details
This workflow is triggered by a Typeform submission and receives feedback text as input.

## Process Summary
The workflow starts when a new form submission is received from Typeform. The submitted feedback text is then analyzed by Google Cloud Natural Language to determine its sentiment score. An If node evaluates the sentiment score from the Google Cloud Natural Language API. If the sentiment score meets a certain condition, a message containing the feedback and its score is posted to a specified Mattermost channel. Otherwise, the workflow proceeds to a NoOp node, signifying no further action.

## Output Details
The workflow either posts a message containing the feedback and sentiment score to a Mattermost channel or completes without external output.

## Tags
automation,n8n,production-ready,excellent,optimized
