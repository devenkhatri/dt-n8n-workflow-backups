# Workflow Analysis for Parse DMARC reports

## Description
This workflow automatically processes DMARC (Domain-based Message Authentication, Reporting, and Conformance) reports received via email, extracts key security and authentication data, stores it in a MySQL database, and optionally sends alerts if issues with DKIM or SPF authentication are detected.

## Input Details
The workflow is triggered by incoming emails containing DMARC reports (typically XML files in ZIP attachments) via an IMAP email account.

## Process Summary
The workflow starts by reading emails with DMARC reports from an IMAP mailbox and downloading their attachments. It then unzips the attachments, extracts XML content, and converts it into JSON format. If the report contains multiple records, it splits them into individual entries. Relevant fields like domain, authentication results, and date ranges are mapped and reformatted for database compatibility. Finally, the parsed data is inserted into a MySQL database table.

## Output Details
The parsed DMARC data is stored in a MySQL database, and (when enabled) failure notifications are sent via Slack or email if DKIM or SPF checks do not pass.

## Tags
DMARC, email security, XML parsing, database, MySQL, automation, n8n, email parsing, SPF, DKIM, security monitoring
