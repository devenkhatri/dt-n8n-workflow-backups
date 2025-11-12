# Workflow Analysis for [OPS] Restore workflows from GitHub to n8n

## Description
This workflow restores n8n workflows that have been backed up to a GitHub repository. It ensures that only workflows not already present in the current n8n instance are recreated, preventing duplicates.

## Input Details
The workflow is triggered manually by clicking 'execute' and uses predefined GitHub repository details (owner, repo name, folder path) set in the Globals node.

## Process Summary
The workflow begins by fetching all workflow files from a specified GitHub repository folder. It decodes their base64 content and extracts workflow names. Separately, it retrieves all existing workflows from the current n8n instance. It then compares the GitHub workflow names with the existing n8n workflow names and keeps only those that don't already exist. Finally, it creates new workflows in n8n using the content and names from GitHub.

## Output Details
The workflow creates new workflows in the n8n instance for each non-duplicate workflow found in the GitHub repository.

## Tags
automation, n8n, GitHub, workflow restoration, backup recovery, production-ready, excellent, optimized
