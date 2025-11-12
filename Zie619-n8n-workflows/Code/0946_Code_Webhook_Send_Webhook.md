# Workflow Analysis for Analyze Email Headers for IPs and Spoofing

## Description
This workflow analyzes email headers to detect potential security threats by extracting IP addresses and checking email authentication protocols like SPF, DKIM, and DMARC. It assesses the reputation of sending IPs using external APIs and provides a detailed report on possible spoofing or spam activity.

## Input Details
The workflow is triggered by a POST webhook that receives raw email headers as plain text in the request body.

## Process Summary
First, the workflow parses the email header string into structured data. It then checks for 'received' headers to extract IP addresses, which are individually analyzed using IP reputation APIs (IP Quality Score and IP-API) to determine fraud risk, abuse history, and geolocation. Separately, it inspects 'authentication-results' and other relevant headers to evaluate SPF, DKIM, and DMARC authentication statuses. The workflow combines both analyses into a unified JSON response containing IP reputation details and email authentication results.

## Output Details
The workflow returns a JSON-formatted response via the webhook containing IP analysis (fraud score, ISP, abuse status, etc.) and email authentication results (SPF, DKIM, DMARC statuses).

## Tags
email security, IP analysis, spoofing detection, phishing protection, email authentication, SPF, DKIM, DMARC, fraud detection, n8n automation
