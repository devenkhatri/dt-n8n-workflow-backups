# Workflow Analysis for Generate Upwork Application Proposal

## Description
This workflow automates the creation of tailored Upwork application proposals for an automation specialist applying to freelance jobs.

## Input Details
The workflow is triggered by an external workflow and receives an Upwork job description as a query.

## Process Summary
The workflow starts by receiving an Upwork job description. It then sets a variable containing detailed information about the automation specialist's experience and achievements. An OpenAI model (GPT-4o-mini) is subsequently used to generate a personalized job proposal, leveraging the job description, the specialist's background, and a specific proposal template. Finally, the generated proposal is extracted from the OpenAI model's response.

## Output Details
The workflow produces a customized Upwork job proposal string.
