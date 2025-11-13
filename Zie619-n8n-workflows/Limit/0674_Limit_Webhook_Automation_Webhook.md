# Workflow Analysis for Gmail Header Analysis Workflow

## Description
This workflow analyzes email headers to determine email authenticity, sender reputation, and geographical origin. It extracts crucial information like SPF, DKIM, and DMARC authentication results, identifies the originating IP address, and queries external APIs for IP quality and location data.

## Input Details
The workflow is triggered by an HTTP POST request to a webhook endpoint, receiving email headers in its body.

## Process Summary
1. The workflow receives email headers via a webhook.
2. It extracts the most relevant 'Received' header to identify the originating IP address, filtering out private IPs.
3. If an IP is found, it queries an IP Quality Score API for sender reputation and an IP API for geographical details like organization, country, and city.
4. It then checks for and extracts 'Authentication-Results', 'Received-SPF', 'DKIM-Signature', and 'DMARC' headers, determining their respective pass/fail/neutral/error/unknown/not found statuses.
5. All extracted and analyzed data, including IP details, spam activity, IP reputation, and authentication results, are merged and aggregated.
6. Finally, the collected information is formatted into a structured JSON object.

## Output Details
The workflow responds to the initiating webhook with a comprehensive JSON object containing the email header analysis, including IP information, sender reputation, and SPF, DKIM, and DMARC authentication statuses.

## Tags
email, header analysis, security, authentication, SPF, DKIM, DMARC, IP reputation, webhook, automation, Gmail
