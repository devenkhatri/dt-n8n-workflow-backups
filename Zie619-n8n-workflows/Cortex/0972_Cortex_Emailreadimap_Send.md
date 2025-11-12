# Workflow Analysis for Email

## Description
This workflow automatically processes incoming emails by extracting attachments, creating security cases in TheHive, analyzing them with Cortex for potential threats like malicious domains, email addresses, or IP addresses, and enriching the case with threat intelligence from external analyzers.

## Input Details
The workflow is manually triggered and fetches emails from an IMAP email account.

## Process Summary
The workflow starts by reading an email from an IMAP account and extracting its first attachment. It creates an observable in TheHive with the attachment, promotes it to a full case, and retrieves the case details. It then fetches observables associated with the case and runs a Cortex analyzer on the file attachment to detect indicators of compromise (IOCs). If any IOCs (domains, emails, or IPs) are found, they are added to the case as observables. Additional analyzers are then run on each IOC type for further threat intelligence enrichment.

## Output Details
The workflow creates and updates a security case in TheHive with enriched threat intelligence data derived from email attachments and their extracted IOCs.

## Tags
email security, threat intelligence, TheHive, Cortex, IOCs, malware analysis, incident response, automation, n8n
