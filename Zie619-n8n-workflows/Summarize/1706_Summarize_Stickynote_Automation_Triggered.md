# Workflow Analysis for Jira Retrospective

## Description
This workflow automates the creation of "Lessons Learned" reports for Jira Epics that have been marked as "Done".

## Input Details
The workflow is triggered by an update to a Jira issue, specifically when an Epic's status changes to "Done".

## Process Summary
The workflow first identifies if a Jira Epic has been completed. If an Epic is "Done", it then fetches all related issues and their comments from Jira. This collected data, including the Epic's name, status, title, description, and concatenated comments, is then fed into an AI agent. The AI agent processes this information and generates a detailed "Lessons Learned" report in Markdown format.

## Output Details
The generated "Lessons Learned" report is then inserted into a specified Google Docs document.

## Tags
automation, n8n, production-ready, excellent, optimized, jira, retrospective, google docs, AI, report generation
