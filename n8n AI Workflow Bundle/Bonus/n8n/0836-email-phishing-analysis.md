# Workflow Analysis for Email Phishing Analysis

## Description
This workflow analyzes suspicious emails for phishing attempts and provides a summary of its findings.

## Input Details
This workflow is triggered manually and does not receive any specific input data initially, but it processes email content provided during execution.

## Process Summary
The workflow starts by clearing any previous phishing data. It then extracts key information from the email, including sender, subject, and body. This information is then compiled into a structured message and sent for analysis using an AI model. Finally, the analysis results are merged with the original email data for a comprehensive report.

## Output Details
The workflow outputs a comprehensive analysis of the suspicious email, including identified phishing indicators, from an AI model.
