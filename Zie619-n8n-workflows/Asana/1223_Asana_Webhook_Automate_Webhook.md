# Workflow Analysis for Production Workflow

## Description
This workflow receives task creation requests via a webhook and automatically creates a new task in Asana using the provided data, then returns a confirmation message with the task's URL.

## Input Details
The workflow is triggered by an incoming HTTP webhook request that includes a 'query.parameter' field used as the Asana task name.

## Process Summary
The workflow starts with a webhook node that listens for incoming requests. It then passes the received data to the Asana node, which creates a new task in Asana using the value from 'query.parameter' as the task name. After the task is created, the Set node constructs a response message containing the Asana task's permalink URL. If any step fails, the workflow routes to an error handler that stops execution and returns an error message.

## Output Details
The workflow outputs a custom message containing the URL of the newly created Asana task, which is returned as the webhook response.

## Tags
asana, task-automation, webhook, production, error-handling
