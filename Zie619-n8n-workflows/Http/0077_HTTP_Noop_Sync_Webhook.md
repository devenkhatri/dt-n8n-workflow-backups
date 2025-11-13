# Workflow Analysis for Syncro Alert to OpsGenie

## Description
This workflow integrates Syncro monitoring alerts with OpsGenie to automatically create or close incidents based on whether an issue is active or resolved.

## Input Details
The workflow is triggered by a POST webhook from Syncro that includes alert data such as computer name, customer info, alert status, and description.

## Process Summary
The workflow first receives a webhook from Syncro. It then checks if the alert trigger is 'agent_offline_trigger' using a Switch node. If so, it evaluates whether the alert is resolved using an IF condition. If the alert is not resolved, it creates a new OpsGenie alert with relevant details. If the alert is resolved, it closes the corresponding OpsGenie alert. A NoOp node handles cases that don't match the trigger condition.

## Output Details
The workflow either creates a new alert or closes an existing one in OpsGenie via HTTP requests using authenticated API calls.

## Tags
Syncro, OpsGenie, alerting, incident management, webhook, automation, IT monitoring, production-ready
