# Workflow Analysis for Email Capture Flow

## Description
This workflow captures email addresses submitted through a website form, validates them with Hunter.io, and then saves valid emails to a GSheet while sending an email notification to the submitter.

## Input Details
The workflow is triggered by an HTTP POST request, typically from a website form submission.

## Process Summary
The workflow starts by receiving an email address from an HTTP POST request. It then validates this email address using Hunter.io to ensure deliverability and checks the verification status. If the email is valid, it appends the email, current date, and a "Verified" status to a Google Sheet. Simultaneously, it sends a confirmation email to the newly captured email address. If the email is invalid according to Hunter.io, it appends the email, current date, and an "Invalid" status to the Google Sheet.

## Output Details
The workflow updates a Google Sheet with captured email addresses and sends a confirmation email to valid submitters.
