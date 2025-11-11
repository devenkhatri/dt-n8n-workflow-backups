# Workflow Analysis for Google Drive Duplicate File Handler

## Description
This workflow automatically detects and manages duplicate files in a specified Google Drive folder. It can either flag duplicates by renaming them with a 'DUPLICATE-' prefix or move them to the trash, while keeping either the first or last version of each file based on configuration.

## Input Details
The workflow is triggered when a new file is created in a specified Google Drive folder, and it receives file metadata including name, ID, owner, folder, creation time, and MD5 checksum.

## Process Summary
The workflow starts by capturing file creation events in a specific Google Drive folder. It then retrieves all files in that folder owned by the same user and filters out Google Apps documents. Using MD5 checksums, it identifies duplicates, keeping either the first or last created file based on configuration. Depending on settings, it either flags duplicates by renaming them or sends them to the trash, while avoiding reprocessing already flagged files.

## Output Details
The workflow either renames duplicate files with a 'DUPLICATE-' prefix or moves them to Google Drive trash, leaving the original file intact based on the configured action.

## Tags
google drive, deduplication, file management, automation, duplicate detection, n8n
