# Workflow Analysis for Error Handler send Telegram

## Description
This workflow automatically sends error notifications to a Telegram chat whenever another workflow encounters an error. It includes key details like workflow name, timestamp, execution URL, last executed node, and error message to help with debugging and monitoring.

## Input Details
The workflow is triggered automatically by errors occurring in other workflows that have this workflow configured as their error handler.

## Process Summary
When an error occurs in a monitored workflow, the Error Trigger node captures the error context. The Config node provides the Telegram chat ID. The Telegram node formats a detailed error message using the captured data and sends it to the specified Telegram chat using configured bot credentials. If sending fails, it retries up to three times with a delay. Finally, the workflow stops with an error status to log the handling outcome.

## Output Details
The workflow sends a formatted error notification message to a specified Telegram chat using a Telegram bot.

## Tags
error handling, telegram, notification, monitoring, n8n, automation, production-ready
