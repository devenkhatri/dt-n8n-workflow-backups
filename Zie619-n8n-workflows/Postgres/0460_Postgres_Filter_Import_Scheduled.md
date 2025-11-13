# Workflow Analysis for Postgres Workflow

## Description
Automated workflow that processes data and performs automated tasks in Postgres

## Input Details
The workflow is triggered manually or by a scheduled trigger every 4 hours

## Process Summary
The workflow starts with a manual trigger or a schedule trigger, then it gets all workflows, sets variables for default error workflow and exclusion tag, filters out workflows with the default error exclusion tag, and finally updates the workflow entity in Postgres with the new settings

## Output Details
The workflow produces an updated workflow entity in Postgres

## Tags
postgres,automation,n8n,production-ready,workflow-automation
