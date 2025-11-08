# Workflow Analysis for Backup n8n Workflows to Git Repository

## Description
This workflow automates the process of backing up all existing n8n workflows to a specified Git repository, ensuring that your workflow definitions are safely stored and version-controlled.

## Input Details
The workflow is typically triggered on a schedule or manually, fetching all currently configured n8n workflows.

## Process Summary
The workflow first retrieves a list of all active n8n workflows. For each workflow, it extracts its definition and prepares it for storage. These workflow definitions are then committed as files to the designated Git repository, effectively creating a version-controlled backup of your n8n configurations.

## Output Details
The workflow successfully updates the specified Git repository with the latest versions of all n8n workflow definitions.
