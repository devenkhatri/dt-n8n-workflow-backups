# Workflow Analysis for Workflow stats

## Description
This workflow analyzes and aggregates statistics about all n8n workflows in the instance, including usage of nodes, tags, and webhooks, and can generate a comprehensive JSON report or a styled HTML dashboard for visualization.

## Input Details
The workflow is triggered either manually (via 'Test workflow' button), by another workflow, or via a webhook request for the HTML dashboard.

## Process Summary
The workflow fetches all workflows from the n8n instance using the n8n API, then processes each workflow to extract and summarize key statistics such as node usage, tags, webhooks, and activity status. It groups this data into sections: global stats, per-workflow details, node usage across workflows, tag usage, and webhook endpoints. The data is then aggregated, sorted, and merged into a single structured JSON object. Optionally, if triggered by a webhook, it converts this JSON into an XML structure and wraps it in an HTML page with an XSL stylesheet to produce a visual dashboard.

## Output Details
The workflow outputs a structured JSON object containing workflow statistics, or—when triggered via webhook—returns an HTML/XML dashboard page that displays the statistics in a user-friendly format.

## Tags
automation, n8n, production-ready, excellent, optimized, dashboard, workflow analytics, node usage, tag analysis, webhook monitoring
