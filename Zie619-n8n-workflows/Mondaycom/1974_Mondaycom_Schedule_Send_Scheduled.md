# Workflow Analysis for Microsoft Outlook AI Email Assistant

## Description
This automated workflow serves as a Microsoft Outlook AI Email Assistant. It integrates with various services to intelligently categorize and prioritize incoming emails, ensuring efficient email management. It includes comprehensive error handling, security measures, and is optimized for production use.

## Input Details
The workflow is triggered manually for testing or by a schedule to periodically check for new emails in Microsoft Outlook. It also receives contact information from Monday.com and categorization rules, categories, and delete rules from Airtable.

## Process Summary
First, the workflow updates contacts in Airtable by retrieving them from Monday.com. It then fetches new, unflagged, and uncategorized emails from Microsoft Outlook. For each email, the body is sanitized by converting it to markdown and removing unnecessary characters, and relevant email fields are extracted. Simultaneously, it retrieves predefined categorization rules, categories, and delete rules from Airtable. An AI agent, utilizing the sanitized email content, contact information, and rules, analyzes and categorizes each email. The AI's output is then parsed to extract the assigned category and subcategory.

## Output Details
The workflow updates the processed emails in Microsoft Outlook by assigning a category and, if determined to be an "Action" item by the AI, sets the email's importance to "High".

## Tags
automation,n8n,production-ready,excellent,optimized,outlook,email,ai,airtable,monday.com
