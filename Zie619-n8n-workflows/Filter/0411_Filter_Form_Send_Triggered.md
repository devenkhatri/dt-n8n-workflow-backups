# Workflow Analysis for Formtrigger Workflow

## Description
This workflow captures leads through a contact form, validates that the submission uses a business email, enriches the lead and their company data using Clearbit, and sends a personalized follow-up email only if the company is a B2B organization with more than 499 employees.

## Input Details
The workflow is triggered by a form submission containing the user's role and business email.

## Process Summary
The workflow starts with a form submission asking for the user's role and business email. It first maps the email field, then filters out common personal email domains. Valid business emails are enriched using Clearbit to get personal and company details. The company data is checked to confirm it is tagged as B2B and has more than 499 employees. If both conditions are met, a personalized thank-you email is sent via Gmail; otherwise, the workflow ends without action.

## Output Details
If criteria are met, a personalized email is sent to the submitter via Gmail; otherwise, no action is taken.

## Tags
lead generation, form automation, email enrichment, Clearbit, Gmail, B2B qualification, workflow automation, n8n
