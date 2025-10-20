# Workflow Analysis for Firestore Document Management

## Description
This workflow demonstrates how to perform various operations (create, update, get, delete) on Firestore documents using webhooks and conditional logic.

## Input Details
The workflow is triggered by an HTTP webhook that receives a JSON payload containing an "operation" field and data.

## Process Summary
First, the workflow checks the "operation" field from the webhook payload. If the operation is "create", it creates a new document in the "n8n_test" collection. If the operation is "update", it updates an existing document based on the provided ID. If the operation is "get", it retrieves a document by its ID. If the operation is "delete", it deletes a document by its ID.

## Output Details
The workflow returns an HTTP 200 success response with the result of the Firestore operation.
