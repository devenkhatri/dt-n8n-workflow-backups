# Workflow Analysis for Automated Phishing Email Reporting to Jira with AI Analysis

## Description
This workflow automates the process of identifying and reporting potential phishing emails. It monitors incoming emails, captures their visual representation, uses AI to analyze the content and headers for phishing indicators, and then automatically creates a detailed Jira ticket for security teams, including an analysis report and a screenshot of the email.

## Input Details
The workflow is triggered by new emails received in a configured Gmail account, polling every minute for new messages.

## Process Summary
The workflow is initiated upon the arrival of a new email in Gmail, extracting its HTML body, subject, recipient, and headers. The extracted email HTML content is then used to generate a screenshot via the hcti.io API, which is subsequently retrieved. An AI model (ChatGPT-4) analyzes the generated screenshot and the email's headers to assess whether it is a phishing attempt. The AI's analysis, along with key email details such as the subject and text body, are compiled into a comprehensive report. Finally, a Jira ticket is automatically created, containing the email information, the AI's phishing analysis, and the generated email screenshot as an attachment.

## Output Details
The workflow creates a new Jira task containing the reported email's subject, recipient, body, a detailed AI-generated phishing analysis, and an attached screenshot of the email.
