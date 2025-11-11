# Workflow Analysis for Webhook Workflow

## Description
This workflow demonstrates how to manage and persist an access token using workflow static data, refreshing it when expired. It supports both webhook and scheduled triggers to ensure the token stays valid for integrations.

## Input Details
The workflow is triggered either by an incoming webhook request or a scheduled trigger, and it accesses existing static data containing an access token and its timestamp.

## Process Summary
The workflow starts by initializing static data with an access token and timestamp if they don't already exist. It then checks if the current token is still valid (not older than 1 minute). If valid, it proceeds without changes. If expired, it makes an HTTP request to fetch a new access token, then updates the static data with the new token and current timestamp.

## Output Details
The workflow updates the global static data with a fresh access token and timestamp when needed, enabling other workflows or steps to use a valid token without redundant authentication calls.

## Tags
access token management, static data, webhook, schedule trigger, authentication, n8n, workflow automation
