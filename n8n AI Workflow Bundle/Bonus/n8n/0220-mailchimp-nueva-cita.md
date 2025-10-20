# Workflow Analysis for Mailchimp New Appointment Automation

## Description
This workflow automates the process of adding new appointment contacts to a Mailchimp audience and sending a welcome email.

## Input Details
The workflow is triggered by an HTTP POST request containing new appointment data.

## Process Summary
The workflow starts by receiving new appointment data via a webhook. It then extracts the client's email, name, and phone number from the received data. Next, it formats the client's name for Mailchimp and adds the client as a new contact to a specified Mailchimp audience. Finally, a welcome email is sent to the newly added contact.

## Output Details
The workflow updates a Mailchimp audience by adding a new contact and sends a welcome email to that contact.
