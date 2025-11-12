# Workflow Analysis for Workflow dashboard with mermaid.js

## Description
This workflow creates a visual dashboard of all n8n workflows using Mermaid.js flowcharts. It allows users to view a list of workflows and dynamically load and render their node-based diagrams in a web interface.

## Input Details
The workflow is triggered either manually or via a webhook, which may include a query parameter 'wfid' to request a specific workflow diagram.

## Process Summary
The workflow begins by checking if a specific workflow ID (wfid) is provided in the query. If not, it fetches a list of all workflows, formats them for display, and returns an HTML dashboard page that lists all workflows with buttons to show their diagrams. If a workflow ID is provided, it fetches the specific workflow details, processes its nodes using custom JavaScript logic to generate a Mermaid.js flowchart (excluding sticky notes and handling node shapes and connections), and returns the diagram as plain text. The dashboard HTML embeds logic to dynamically fetch and render Mermaid diagrams via additional webhook calls.

## Output Details
The workflow returns either a full HTML dashboard page listing all workflows or a Mermaid.js diagram as plain text, depending on the input, both served via webhook responses.

## Tags
automation, n8n, production-ready, excellent, optimized, dashboard, mermaid.js, workflow visualization, webhook, html
