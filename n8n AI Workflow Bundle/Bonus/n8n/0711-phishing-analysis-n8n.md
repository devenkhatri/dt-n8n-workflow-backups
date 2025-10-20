# Workflow Analysis for Phishing Email Analysis and Reporting

## Description
This workflow automates the analysis of potential phishing emails, extracts key information, and generates a detailed report, enabling rapid response to security threats.

## Input Details
This workflow is triggered manually by an HTTP request that provides the email content as input.

## Process Summary
The workflow starts by receiving an email via a webhook. It then extracts specific elements from the email, such as the subject and sender details. Subsequently, it uses a large language model to analyze the email content for phishing indicators and categorize it. Finally, it formats the extracted information and AI analysis into a structured report.

## Output Details
The workflow generates a structured JSON report containing a phishing analysis, including the sender, subject, analysis results, and a conclusion, which is then returned as an HTTP response.
