# Workflow Analysis for Automate SIEM Enrichment with MITRE ATT&CK

## Description
This workflow automates the enrichment of Security Information and Event Management (SIEM) data by cross-referencing indicators of compromise (IOCs) with the MITRE ATT&CK framework database. It helps security analysts to quickly understand the context and potential threats associated with security events, improving incident response and threat intelligence.

## Input Details
This workflow is manually triggered and designed to process a JSON array of indicators of compromise (IOCs) as input.

## Process Summary
First, the workflow extracts and processes each IOC from the input JSON. It then queries the MITRE ATT&CK database to find matching tactics, techniques, and procedures (TTPs) for each IOC. Next, it formats the MITRE ATT&CK data into a readable format. Finally, it combines the original IOC data with the enriched MITRE ATT&CK information.

## Output Details
The workflow outputs a JSON array, with each object containing the original IOC and its corresponding enriched MITRE ATT&CK information.
