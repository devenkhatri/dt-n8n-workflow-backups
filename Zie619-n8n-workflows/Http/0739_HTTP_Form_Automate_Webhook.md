# Workflow Analysis for Streamline Your Zoom Meetings with Secure, Automated Stripe Payments

## Description
This workflow automates the end-to-end process of creating a Zoom meeting, setting up a Stripe payment product and link, storing event details in Google Sheets, and sending personalized email notifications to both the event organizer (teacher) and participants upon successful payment.

## Input Details
The workflow is triggered by a web form submission that collects event details (title, price, start date, hour, and minute).

## Process Summary
When a new event is submitted via the creation form, the workflow creates a Zoom meeting and a corresponding Stripe product. It then generates a secure Stripe payment link with embedded Zoom details and event metadata. A new Google Sheet tab is created to track participants for this event. Finally, the teacher receives an email with the payment link, Zoom access details, and a link to the participant list. A separate branch (currently disabled) handles incoming Stripe payment webhooks to register participants and notify both the participant and the teacher.

## Output Details
The workflow outputs a Zoom meeting, a Stripe payment link, a dedicated Google Sheet tab for participant registration, and sends confirmation emails to both the teacher and participants.

## Tags
Zoom, Stripe, Google Sheets, Gmail, automation, payment processing, event management, webinar, n8n
