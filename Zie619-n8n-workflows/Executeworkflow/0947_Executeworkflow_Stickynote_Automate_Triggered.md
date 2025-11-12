# Workflow Analysis for Workflow Results to Markdown Notes in Your Obsidian Vault, via Google Drive

## Description
This workflow automatically converts results from any n8n workflow into well-structured Markdown notes with optional YAML frontmatter and saves them to a Google Drive folder that syncs with your Obsidian Vault using a symbolic link. It also supports saving binary attachments alongside the notes.

## Input Details
The workflow is triggered by receiving JSON data from another n8n workflow via an Execute Workflow Trigger node.

## Process Summary
The workflow first checks if the input contains binary attachments. If so, it saves those to Google Drive. Separately, it can optionally use AI (via OpenAI nodes) to transform the input into a structured Zettlekasten-style note and generate YAML frontmatter. The final note data is restructured into title, content, and frontmatter fields, then saved as a Markdown (.md) file in a designated Google Drive folder.

## Output Details
The workflow produces Markdown files (and optionally binary attachments) saved in a Google Drive folder that is symlinked to an Obsidian Vault, making the notes instantly available in Obsidian.

## Tags
obsidian, markdown, google drive, zettlekasten, ai notes, knowledge management, n8n, automation, workflow integration
