# Workflow Analysis for Affected Workflows Detector

## Description
This workflow helps identify n8n workflows that may have been incorrectly rewired due to a bug in version 0.214.3, specifically affecting nodes with multiple outputs like 'If', 'Switch', and 'Compare Datasets'. It generates an HTML report listing potentially impacted workflows and nodes for manual review.

## Input Details
The workflow is triggered by an HTTP GET request to the '/webhooks/affected-workflows' endpoint and fetches all workflows from the n8n instance via the n8n API using configured credentials.

## Process Summary
The workflow starts with a webhook trigger. It then uses the n8n API node to fetch all workflows in the instance. A code node processes each workflow to detect multi-output nodes (like 'If' or 'Switch') that may have missing or misrouted connections due to a past migration bug. It compiles a list of workflows with potentially affected nodes. Finally, it generates and serves an interactive HTML report via a webhook response, listing each affected workflow with clickable links to inspect them.

## Output Details
The workflow produces an HTML report served directly to the user’s browser, listing all potentially affected workflows with links to open them in the n8n editor for verification.

## Tags
n8n, workflow-audit, bug-detection, multi-output-nodes, automation, html-report, webhook-trigger
