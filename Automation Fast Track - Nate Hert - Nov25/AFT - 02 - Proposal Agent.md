# Workflow Analysis for AFT - 02 - Proposal Agent

## Description
This workflow automatically generates a client proposal after a sales call by extracting key information from a Fathom call recording, retrieving lead details from Google Sheets, and populating a Google Slides proposal template with AI-generated content based on the call transcript.

## Input Details
The workflow is triggered by a POST webhook that receives call recording data from Fathom, including transcript, attendees, summary, and metadata.

## Process Summary
The workflow starts by capturing the Fathom call recording data via a webhook. It then retrieves the lead's information from a Google Sheets CRM using the attendee's email. If the call is a sales call (determined by checking if the 'Sales Transcript ID' is empty), it cleans and formats the transcript, then uses an AI model to extract structured proposal content like problem bottlenecks, solutions, project phases, and pricing. It copies a Google Slides proposal template, replaces placeholders with the extracted content, sends the proposal via Gmail for internal review, and updates the CRM sheet to mark the proposal as sent and record the call ID.

## Output Details
The workflow produces a customized Google Slides proposal document, sends it via email for internal review, and updates the lead's record in Google Sheets with the proposal status and call transcript ID.

## Tags
proposal generation, sales automation, AI extraction, Fathom integration, Google Workspace, CRM update, workflow automation
