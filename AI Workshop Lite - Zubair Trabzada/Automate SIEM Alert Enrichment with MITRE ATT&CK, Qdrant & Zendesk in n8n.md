# Workflow Analysis for Automated SIEM Alert Enrichment with MITRE ATT&CK and Qdrant

## Description
This workflow automates the enrichment of SIEM (Security Information and Event Management) alerts by querying MITRE ATT&CK information from a Qdrant vector database and creating tickets in Zendesk.

## Input Details
The workflow is triggered manually and receives an alert name as input.

## Process Summary
The workflow starts by taking an alert name as input. It then queries a Qdrant vector database to retrieve MITRE ATT&CK information related to the alert. After processing the retrieved data, it creates a new ticket in Zendesk, populating it with the alert details and the enriched MITRE ATT&CK information. Finally, it sends a message to a Discord channel confirming the ticket creation.

## Output Details
The workflow creates a Zendesk ticket with enriched alert details and sends a confirmation message to Discord.
