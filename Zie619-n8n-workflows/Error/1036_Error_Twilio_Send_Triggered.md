# Workflow Analysis for Send an SMS when a workflow fails

## Description
This workflow automatically sends an SMS notification whenever another workflow in the system fails, providing immediate visibility into errors for faster troubleshooting.

## Input Details
The workflow is triggered automatically by any workflow failure within the n8n system and receives error metadata including the failed workflow’s ID and name.

## Process Summary
The workflow starts with an Error Trigger node that activates when any workflow fails. It captures details about the failed workflow, such as its ID and name. These details are then used to compose an SMS message via the Twilio node, which sends the alert to a predefined phone number. An Error Handler node is included to manage any exceptions during execution.

## Output Details
The workflow sends an SMS message via Twilio containing the ID and name of the failed workflow.

## Tags
error handling, SMS alert, workflow monitoring, Twilio, automation, n8n, production-ready
