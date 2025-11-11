# Workflow Analysis for Error Logger

## Description
This workflow automatically captures and logs errors from other n8n workflows, recording key details like timestamp, workflow name, failing node, and error message into a Google Sheet, while optionally sending a real-time alert to a Slack channel.

## Input Details
The workflow is triggered automatically whenever any other workflow in the n8n instance encounters an error, receiving error metadata including workflow name, execution URL, node name, and error message.

## Process Summary
The workflow starts with an Error Trigger that activates on any workflow failure. It simultaneously logs the error details—such as timestamp, workflow name, execution URL, failing node, and error message—into a specified Google Sheet. At the same time, it sends a formatted error notification to a designated Slack channel. The Google Sheet and Slack channel must be pre-configured with valid credentials. The workflow acts as a global error handler for the n8n environment.

## Output Details
The workflow outputs error records to a Google Sheet and sends real-time error notifications to a Slack channel.

## Tags
error handling, logging, Google Sheets, Slack, monitoring, alerting, workflow automation
