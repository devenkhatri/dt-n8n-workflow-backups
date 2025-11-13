# Workflow Analysis for Wordpress Form to Mautic

## Description
When a WordPress form is submitted, the workflow receives the form data via a webhook, normalizes and validates the email address, and then either creates a new contact in Mautic with the provided details or flags the entry as Do Not Contact if the email is invalid.

## Input Details
The workflow is triggered by a POST webhook from a WordPress form that sends fields such as Nome, E‑mail, WhatsApp and form identifiers.

## Process Summary
1) The webhook captures the raw form submission. 2) A Set node formats the name, lower‑cases the email, extracts the mobile number and checks email validity. 3) An IF node routes the data based on whether the email is valid. 4) Valid emails trigger a Mautic node that creates a new contact with the name, email and mobile. 5) Invalid emails trigger a Mautic node that adds the entry to the Do Not Contact list with a reason, and the workflow ends.

## Output Details
Creates a new contact in Mautic for valid emails or updates the contact's Do Not Contact status for invalid emails, then finishes execution.

## Tags
automation,wordpress,mautic,webhook,email validation,lead capture
