# Workflow Analysis for Production Workflow

## Description
Production-ready workflow: Production Workflow. This workflow has been optimized for production use with comprehensive error handling, security, and documentation.

## Input Details
This workflow is triggered by a POST request to a webhook endpoint and receives student and event type data in its body.

## Process Summary
The workflow is triggered by a POST webhook, extracting student and type data. It then splits the student's full name into first and last names if provided. The workflow branches based on the type: for User types, it finds or creates a contact in Mautic, then updates contact details, unsubscribes, or subscribes based on further User.type specifics. For Sale types, it finds the relevant user in Mautic. Finally, it tags the user in Mautic with the course name from the incoming data.

## Output Details
The workflow creates new contacts, updates existing contacts, or adds/removes tags for contacts in Mautic.

## Tags
automation,n8n,production-ready,excellent,optimized
