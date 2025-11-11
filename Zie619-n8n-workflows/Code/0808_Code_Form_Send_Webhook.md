# Workflow Analysis for Website Security Scanner

## Description
This workflow scans a website URL for security vulnerabilities by analyzing HTTP headers and page content, then generates and emails a detailed security audit report with a letter grade and remediation advice.

## Input Details
The workflow is triggered by a form submission containing a website URL to scan.

## Process Summary
The workflow starts by accepting a URL via a web form. It then fetches the website’s HTML and HTTP headers using an HTTP request. Two parallel analyses are performed using OpenAI: one examines security headers and configuration, while the other scans the HTML/JavaScript for client-side vulnerabilities like XSS. The results from both analyses are merged, processed to calculate a security grade (A-F), and formatted into a professional HTML email report. Finally, the report is sent via Gmail to a predefined recipient.

## Output Details
The workflow produces a comprehensive HTML-formatted security audit report and sends it via email using Gmail.

## Tags
website security, vulnerability scanner, security audit, HTTP headers analysis, XSS detection, OpenAI, Gmail integration, form trigger, n8n workflow, automated reporting
