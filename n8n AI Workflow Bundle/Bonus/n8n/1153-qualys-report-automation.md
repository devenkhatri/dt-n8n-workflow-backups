# Workflow Analysis for Qualys Report Automation

## Description
This workflow automates the generation and distribution of Qualys asset reports. It retrieves asset data, generates a report, and sends it to specified recipients via email and Microsoft Teams.

## Input Details
The workflow is triggered manually.

## Process Summary
The workflow starts manually to retrieve the details of the assets from the Qualys platform. Then the workflow creates a CSV file containing the retrieved asset data. After that, it converts the CSV file into a base64 encoded string. Next, an email with the CSV attachment containing the asset details is sent to the configured recipients via Gmail. Finally, the same CSV file with asset data is also sent as a message to a Microsoft Teams channel.

## Output Details
The workflow sends an email with the Qualys asset report as a CSV attachment via Gmail and posts the same report to a Microsoft Teams channel.
