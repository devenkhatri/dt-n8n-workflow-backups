# Workflow Analysis for Unsubscribe Mautic contacts from automated unsubscribe emails

## Description
Automated workflow: Unsubscribe Mautic contacts from automated unsubscribe emails. This workflow integrates 7 different services: stickyNote, mautic, code, gmailTrigger, set. It contains 16 nodes and follows best practices for error handling and security.

## Input Details
The workflow is triggered by new emails received in a configured Gmail account, checking for new messages every minute.

## Process Summary
First, the workflow sets a predefined email address and an unsubscribe message. It then checks if the incoming email is an automated unsubscribe request and not sent from the predefined email address. If conditions are met, it extracts unique email addresses from the sender's "From" field. Next, it searches for these email addresses in Mautic to retrieve contact IDs. If a contact exists in Mautic, the workflow adds them to an "unsubscribed" segment and removes them from the "newsletter" segment. Optionally, it can also add them to a "Do Not Contact List". Finally, it replies to the original email with the predefined unsubscribe message.

## Output Details
The workflow updates contact segments in Mautic by adding contacts to an unsubscribed segment and removing them from a newsletter segment, and sends a reply email confirming the unsubscribe to the sender.

## Tags
automation,n8n,production-ready,excellent,optimized
