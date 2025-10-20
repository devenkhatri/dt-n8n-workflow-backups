# Workflow Analysis for Phishing Email Analysis and Reporting

## Description
This workflow analyzes suspicious emails for phishing attempts, extracts key information, and reports potential threats to a security team via Discord. It leverages AI to summarize email content and assess phishing likelihood.

## Input Details
The workflow is triggered manually by a user and requires a suspicious email as input.

## Process Summary
The workflow begins by extracting email details such as sender, recipient, subject, and body. It then uses an AI model to summarize the email content and determine the likelihood of it being a phishing attempt. If the email is flagged as phishing, the workflow sends a formatted alert to a Discord channel, including a summary and key indicators. Finally, it provides a confirmation message indicating whether the email was analyzed and, if applicable, reported as phishing.

## Output Details
The workflow sends potential phishing alerts to a Discord channel and provides a confirmation message to the user.
