# Workflow Analysis for Automated Lead Generation and Outreach with AI

## Description
This workflow automates lead generation, enriches lead data using AI, and initiates personalized outreach via email.

## Input Details
The workflow is triggered manually by clicking "Execute Workflow".

## Process Summary
The workflow starts by manually creating lead data as a JSON. It then uses the OpenAI API to categorize interests based on the provided lead data. Following this, the workflow generates a personalized cold email draft using OpenAI, incorporating the lead's company name, interests, and a call to action. Finally, it uses Gmail to send the generated cold email to the lead, dynamically pulling the recipient's email address, subject, and body from the previous steps.

## Output Details
The workflow sends personalized cold emails to leads via Gmail.
