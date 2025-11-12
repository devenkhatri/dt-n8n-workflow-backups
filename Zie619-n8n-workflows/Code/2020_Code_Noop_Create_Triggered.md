# Workflow Analysis for Addon for Workflow Nodes Update Check Template

## Description
This workflow automatically identifies and handles outdated nodes in n8n workflows. It can optionally add updated node versions to the canvas and rename outdated nodes with a warning symbol, then sends an email summary listing all affected workflows.

## Input Details
The workflow is triggered by another workflow that provides a list of workflows containing outdated nodes, including each workflow’s ID and details about the outdated nodes.

## Process Summary
The workflow starts by receiving input data about outdated nodes in other workflows. It applies user-defined settings such as whether to handle only major version changes and whether to add updated nodes to the canvas. It then fetches each referenced workflow via the n8n API, modifies it by prepending a warning symbol to outdated node names and optionally inserting updated node versions nearby, and saves the updated workflow back via the API. Finally, it compiles a list of affected workflows with clickable links and sends an email summary via Gmail.

## Output Details
The workflow updates the specified n8n workflows in place and sends an email via Gmail listing all workflows that contained outdated nodes, with hyperlinks to each workflow in the n8n editor.

## Tags
n8n, workflow update, node versioning, automation, email alert, workflow maintenance, production-ready
