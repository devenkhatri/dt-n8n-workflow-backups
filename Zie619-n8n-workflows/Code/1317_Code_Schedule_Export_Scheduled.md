# Workflow Analysis for 🧹 Archive (delete) duplicate items from a Notion database

## Description
This workflow automatically identifies and archives (deletes) duplicate pages in a Notion database based on a specified property, ensuring only one unique copy remains.

## Input Details
The workflow is triggered either daily via a schedule or instantly when a new page is added to the Notion database, and it receives the full list of database pages from Notion.

## Process Summary
First, the workflow fetches all pages from a specified Notion database. It then reformats each page to extract a user-defined property for duplicate checking. All pages are aggregated into a single list, which is then processed by a custom JavaScript function to identify duplicates based on the selected property. Finally, the identified duplicate pages are archived (soft-deleted) in Notion.

## Output Details
The workflow archives (deletes) duplicate Notion pages, leaving only the first occurrence of each unique item based on the specified property.

## Tags
Notion, deduplication, automation, data cleaning, archive, duplicate removal, n8n, production-ready
