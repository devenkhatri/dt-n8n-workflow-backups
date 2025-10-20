# Workflow Analysis for Appointment Qualifier AI

## Description
This workflow uses AI to qualify appointments based on a provided appointment summary and a lead profile. It determines if an appointment is qualified, unqualified, or needs follow-up, and extracts key details like the name and an explanation for the decision.

## Input Details
The workflow is triggered by a webhook and receives an appointment summary and a lead profile as input.

## Process Summary
The workflow starts by receiving appointment and lead data via a webhook. It then uses an AI model to analyze the provided appointment summary and lead profile to determine if the appointment is qualified. Based on the AI's output, the workflow categorizes the appointment as "qualified," "unqualified," or "follow-up needed," and extracts the relevant information.

## Output Details
The workflow responds to the webhook with the qualification status of the appointment, the extracted name, and an explanation for the decision.
