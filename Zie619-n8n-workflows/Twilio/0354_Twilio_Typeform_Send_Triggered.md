# Workflow Analysis for Send Typeforms leads via Whatsapp (Twilio)

## Description
This workflow automates the process of capturing new lead submissions from Typeform and instantly sending their details as a WhatsApp message via Twilio.

## Input Details
The workflow is triggered by new form submissions from a specified Typeform form and receives the complete form response data.

## Process Summary
The workflow starts when a new submission is received from a configured Typeform. Next, a "Set" node extracts specific answers from the Typeform submission and formats them into a single descriptive text string. Subsequently, the "Twilio" node sends a WhatsApp message to a predefined number, containing the formatted lead data. An "Error Handler" node is also configured to catch and stop the workflow execution in case of any errors during the process.

## Output Details
The workflow sends a WhatsApp message containing the new lead's information to a specific phone number using Twilio.

## Tags
Typeform, Twilio, WhatsApp, Leads, Automation, Forms, Messaging
