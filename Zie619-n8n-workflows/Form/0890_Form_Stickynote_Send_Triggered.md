# Workflow Analysis for Hubspot Workflow

## Description
This workflow automates the processing of client conversations by summarizing the transcript, saving the summary as a meeting note in HubSpot linked to the client's contact, and routing relevant feedback to the appropriate internal department via email.

## Input Details
The workflow is triggered by a form submission containing the client's email address and a transcript of their conversation.

## Process Summary
First, the workflow captures the client email and conversation transcript via a form. It then searches HubSpot for the contact using the provided email to retrieve the contact ID. The conversation transcript is summarized into 2-3 sentences using an LLM. The summary is added to HubSpot as a new meeting note associated with the client's contact. Separately, an AI-powered router analyzes the transcript to determine which internal department (Support, Admin, Product, or Commercial) should be notified and sends an email via Gmail with the client's message and context.

## Output Details
The workflow saves a summarized meeting note to the client's HubSpot contact record and sends a routed email notification to the relevant internal department.

## Tags
HubSpot, client feedback, meeting notes, email routing, LLM, summarization, automation, CRM, Gmail, form trigger
