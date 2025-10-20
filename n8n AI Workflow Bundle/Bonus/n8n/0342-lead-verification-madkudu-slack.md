# Workflow Analysis for Lead Verification with MadKudu and Slack Integration

## Description
This workflow automates lead verification by leveraging MadKudu for scoring and then uses the results to send targeted notifications via Slack. It helps sales teams prioritize and connect with high-quality leads efficiently.

## Input Details
The workflow is triggered by an HTTP POST request, receiving lead data that typically includes an email address.

## Process Summary
The workflow starts by extracting the email from the incoming lead data. It then queries the MadKudu API to get a score for the provided email. After receiving the MadKudu response, it checks if the account tier is "top" or "good". Based on the tier, it forms a message with relevant lead information and sends it to a designated Slack channel for sales follow-up.

## Output Details
The workflow sends notifications to a Slack channel with lead information, categorized by MadKudu's lead scoring.
