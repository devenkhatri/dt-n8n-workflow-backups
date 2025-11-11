# Workflow Analysis for Qualys Slack Integration Workflow

## Description
This workflow enables users to trigger Qualys vulnerability scans and generate security reports directly from Slack using interactive modals. It processes Slack commands, collects user input through custom modals, and executes corresponding Qualys operations such as starting scans or creating reports in selected formats.

## Input Details
The workflow is triggered by incoming Slack webhook events, specifically from shortcut commands or modal submissions in Slack.

## Process Summary
The workflow starts by receiving a webhook from Slack and parsing the payload. It then routes the request based on the callback ID or modal submission type—either opening a vulnerability scan modal or a report generation modal. When a user submits a modal, the workflow captures the input values, sets required variables, and executes the appropriate sub-workflow to interact with Qualys (either starting a scan or creating a report). All interactions are acknowledged back to Slack to maintain a smooth user experience.

## Output Details
The workflow triggers Qualys vulnerability scans or report creation based on user input, and results are communicated back to Slack channels as configured in sub-workflows.

## Tags
Slack, Qualys, vulnerability scan, security report, webhook, modal, n8n
