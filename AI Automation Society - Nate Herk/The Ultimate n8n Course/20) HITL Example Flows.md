# Workflow Analysis for Human-in-the-Loop (HITL) Data Approval Workflow

## Description
This workflow demonstrates a Human-in-the-Loop (HITL) process where data fetched from a Google Sheet is reviewed by a human user who decides whether to approve or reject the record, with the original sheet being updated accordingly.

## Input Details
The workflow is initiated manually using a Manual Trigger.

## Process Summary
The workflow begins by manually triggering the execution and retrieving all records from a specified Google Sheet. It then processes each record by extracting an ID and sending a review request to a Human-in-the-Loop (HITL) inbox, pausing the execution until a decision is made. A switch node checks the human's action ('approved' or 'rejected'). Based on the decision, the workflow updates the 'Status' column of the original Google Sheet record to the appropriate value, completing the approval cycle.

## Output Details
The workflow updates the 'Status' column (to 'Approved' or 'Rejected') of the corresponding row in the Google Sheet based on the manual review decision.
