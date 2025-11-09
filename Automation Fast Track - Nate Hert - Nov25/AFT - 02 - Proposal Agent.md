# Workflow Analysis for AFT - 02 - Proposal Agent

## Description
This workflow automatically generates a client-specific sales proposal after a sales call is recorded in Fathom. It pulls lead information from a Google Sheet, determines if the call was a sales or closing call, extracts key details from the call transcript using AI, and populates a Google Slides proposal template with structured content like solutions, project phases, and pricing. The generated proposal is then emailed for internal review and the CRM sheet is updated to reflect the new proposal status and call details.

## Input Details
The workflow is triggered by a POST webhook that receives a Fathom call recording payload containing meeting details, transcript, attendees, and action items.

## Process Summary
The workflow starts by capturing the Fathom call transcript via a webhook. It then retrieves the associated lead's information from a Google Sheet using the attendee's email. An 'if' condition checks whether the call is a sales call (by verifying if a Sales Transcript ID is missing). If it's a sales call, the transcript is cleaned and formatted, then passed to an AI model to extract structured proposal content (e.g., bottlenecks, solutions, phases, pricing). This data populates a copied Google Slides proposal template, which is then emailed for review and the CRM sheet is updated with the proposal status and transcript ID. If it's not a sales call (i.e., a closing call), only the latest call ID is updated in the CRM.

## Output Details
The workflow produces a customized Google Slides proposal document, sends it via email for internal review, and updates the lead's record in a Google Sheet with proposal and call tracking information.

## Tags
proposal generation, sales automation, fathom integration, google sheets, google slides, ai extraction, crm update, webhook trigger
