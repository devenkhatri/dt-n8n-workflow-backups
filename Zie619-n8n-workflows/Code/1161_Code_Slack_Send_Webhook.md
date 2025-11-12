# Workflow Analysis for Receive and analyze emails with rules in Sublime Security

## Description
This workflow automatically monitors a designated email inbox for phishing reports, analyzes any attached .eml files using Sublime Security's threat detection rules, and sends a summary of the analysis to a Slack channel. If no attachment is found, it alerts the team via Slack for manual follow-up.

## Input Details
The workflow is triggered when a new email arrives in a configured IMAP inbox (typically a phishing reporting mailbox), and it receives the full email including any attachments.

## Process Summary
The workflow starts by reading emails from an IMAP inbox. It checks if the email contains an .eml attachment. If an attachment is present, it converts the binary data to a base64-encoded JSON format and sends it to Sublime Security's API for analysis against active detection rules. The response is processed to separate matched and unmatched rules, then formatted into a readable message. Finally, the results are posted to a Slack channel. If no attachment is found, a notification is sent to Slack indicating the missing attachment.

## Output Details
The workflow sends a formatted Slack message showing how many security rules matched the email, along with the names of the matched rules; if no attachment is found, it sends an alert to the same Slack channel.

## Tags
email security, phishing detection, Sublime Security, n8n, automation, IMAP, Slack integration, threat analysis, .eml processing, security workflow
