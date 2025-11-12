# Workflow Analysis for Docsify example

## Description
This workflow creates a self-hosted documentation system for n8n workflows using Docsify.js. It automatically generates, displays, and allows editing of Markdown documentation files for each workflow, including Mermaid diagrams of workflow structure and AI-generated descriptions.

## Input Details
The workflow is triggered by HTTP webhook requests to specific file paths (like README.md, docs_{id}.md, or tag-{tag}.md) with optional query parameters like 'action' (view/edit/recreate/save).

## Process Summary
When a request comes in, the workflow first determines the file type and action needed. For workflow documentation requests, it checks if a documentation file already exists. If not, it fetches the workflow details from n8n's API, generates a Mermaid flowchart of the workflow structure, and uses AI (OpenAI) to create descriptive documentation. The system supports viewing existing docs, editing them in a live Markdown editor with preview, and saving changes back to the file system. For the main page, it generates a table listing all workflows with their status, tags, and metadata.

## Output Details
The workflow responds with either HTML pages (for main documentation interface or editor) or Markdown content (for Docsify.js to render), and can save edited documentation files to the local file system.

## Tags
automation, n8n, production-ready, excellent, optimized, documentation, docsify, markdown, workflow-documentation, mermaid-diagrams
