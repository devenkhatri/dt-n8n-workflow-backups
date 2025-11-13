# Workflow Analysis for Lead Generation and Nurturing Workflow

## Description
This workflow automates the process of collecting leads through a form, verifying their email addresses, scoring their customer fit, and then initiating a personalized email outreach and recording the interaction in HubSpot for qualified leads.

## Input Details
The workflow is triggered by an n8n form submission, collecting a business email from the user.

## Process Summary
First, the submitted business email is verified for validity using Hunter. If the email is valid, the lead is then scored for customer fit using MadKudu. If the customer fit score is greater than 60, the workflow proceeds to retrieve contact information from HubSpot. Subsequently, a personalized outreach email is composed and sent via Gmail, and this email engagement is recorded in HubSpot. If the email is invalid or the customer fit score is 60 or less, no further action is taken.

## Output Details
The workflow sends an outreach email to qualified leads via Gmail and records the email engagement as an activity in HubSpot.

## Tags
lead generation, email verification, lead scoring, CRM, email marketing, n8n, automation, hubspot, hunter, madkudu
