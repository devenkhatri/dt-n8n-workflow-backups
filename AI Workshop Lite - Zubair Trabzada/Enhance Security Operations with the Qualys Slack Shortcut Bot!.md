# Workflow Analysis for Qualys Slack Integration Workflow

## Description
This workflow enables security teams to trigger vulnerability scans and generate reports directly from Slack using interactive modals. It integrates Slack with Qualys to streamline security operations by allowing users to initiate scans or create reports without leaving their messaging platform.

## Input Details
The workflow is triggered by incoming webhook requests from Slack, which include interaction payloads such as shortcut triggers or modal form submissions.

## Process Summary
The workflow starts by parsing the incoming Slack webhook payload. It then routes the message based on the interaction type: either opening a modal for vulnerability scans, opening a modal for report generation, or processing a submitted modal. For submissions, it extracts user inputs like scan title, asset groups, report template, and output format, then passes this data to sub-workflows that interact with Qualys to start scans or generate reports. Finally, it sends appropriate responses back to Slack to close modals or confirm actions.

## Output Details
The workflow sends HTTP responses back to Slack to close modals or acknowledge interactions, and triggers sub-workflows that ultimately create vulnerability scans or generate and share Qualys reports in Slack channels.

## Tags
Slack, Qualys, vulnerability scan, security automation, report generation, webhook, modal, workflow automation
