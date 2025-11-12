# Workflow Analysis for Formtrigger Workflow

## Description
This workflow automates the process of scheduling appointments through a multi-step form experience. It collects user details and enquiry, validates the request using AI, presents terms and conditions, collects preferred date/time, and then sends a confirmation to the user while initiating an internal approval process. Once approved by an admin, it creates a Google Calendar event; if rejected, it notifies the user accordingly.

## Input Details
The workflow is triggered by a web form submission containing the user's name, email, and enquiry.

## Process Summary
The workflow starts by collecting user information via a form. It uses AI to classify whether the enquiry warrants an appointment—if not, the user is redirected to contact via email instead. If valid, the user proceeds through additional forms to accept terms and select a date/time. After submission, the user receives an acknowledgment email, and a separate sub-workflow sends an approval request to an admin. Based on the admin's response (approve/decline), the workflow either creates a Google Calendar event with a meeting link or sends a rejection email to the user.

## Output Details
The workflow sends confirmation or rejection emails to the user, creates a Google Calendar event if approved, and notifies the admin for approval via Gmail with interactive buttons.

## Tags
appointment scheduling, form automation, AI classification, Gmail integration, Google Calendar, approval workflow, multi-step forms, n8n workflow
