# Workflow Analysis for Microsoftoutlooktrigger Workflow

## Description
This workflow analyzes email headers to assess an email's legitimacy and sender reputation. It extracts critical information like the originating IP address and checks email authentication protocols (SPF, DKIM, DMARC) to help identify potential spam or spoofing.

## Input Details
The workflow is primarily triggered by an HTTP POST request to a webhook, receiving email header data from a third-party platform.

## Process Summary
1. The workflow is triggered by an HTTP POST request containing email headers. 2. It extracts and processes "Received" headers to identify and clean the original sender's IP address. 3. The extracted IP address is then used to query external services for IP quality score, organization, and geographic details. 4. The workflow checks for "Authentication-Results", "Received-SPF", "DKIM-Signature", and "DMARC" headers, extracting and evaluating their values to determine email authentication statuses. 5. All collected data, including IP details and authentication results, are consolidated and formatted into a structured output.

## Output Details
The workflow produces a structured JSON response containing the email authentication results, originating IP details, and sender reputation, which is sent back to the calling system via the webhook.

## Tags
automation,n8n,production-ready,excellent,optimized
