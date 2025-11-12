# Workflow Analysis for Formtrigger Workflow

## Description
This workflow automates the appointment scheduling process using multi-step forms, AI-based enquiry classification, and human-in-the-loop approval. It collects user details, validates the request using AI, gathers availability, sends a confirmation receipt, and waits for admin approval before creating a calendar event or notifying the user of rejection.

## Input Details
The workflow is triggered by a web form submission containing the user's name, email, and enquiry details.

## Process Summary
The workflow begins by collecting the user's name, email, and enquiry via a form. It uses AI to classify whether the enquiry is relevant enough to warrant an appointment; if not, the user is redirected to contact via email instead. If relevant, the user proceeds through additional forms to accept terms and select a preferred date and time. After submission, a confirmation email is sent to the user, and a separate sub-workflow triggers an approval request to an admin via email. Based on the admin's response (approve or decline), the workflow either creates a Google Calendar event with a meeting link or sends a rejection email to the user.

## Output Details
The workflow outputs either a scheduled Google Calendar event with an email confirmation or a rejection email to the requester, depending on admin approval.

## Tags
appointment scheduling, form automation, AI classification, human approval, Google Calendar, Gmail integration, multi-step forms, workflow automation
