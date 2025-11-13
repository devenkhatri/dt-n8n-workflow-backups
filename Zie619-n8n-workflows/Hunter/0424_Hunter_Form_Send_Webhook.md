# Workflow Analysis for Formtrigger Workflow

## Description
This automated workflow processes contact form submissions to qualify leads. It integrates email verification, lead scoring, and conditional alerting to identify and notify about high-potential customers.

## Input Details
The workflow is triggered by submissions to an n8n contact form, receiving a business email address as input.

## Process Summary
First, a user submits their business email through a contact form. Then, the workflow verifies the email's validity using Hunter. If the email is valid, it proceeds to score the lead's customer fit using MadKudu. Finally, if the customer fit score is above 60, an alert email is sent.

## Output Details
The workflow sends an email alert via Gmail to a specified recipient with details about "hot leads" that have a customer fit score greater than 60.

## Tags
automation,n8n,production-ready,excellent,optimized
