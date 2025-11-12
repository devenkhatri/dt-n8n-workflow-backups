# Workflow Analysis for Batch File Upload to Google Drive

## Description
This workflow allows users to upload multiple files to a specific Google Drive folder via a form. If the folder doesn't exist, it automatically creates one with the provided name and uploads all files into it, preserving original file names.

## Input Details
The workflow is triggered by a form submission that includes one or more files and a target folder name.

## Process Summary
The workflow starts by capturing form input with files and a folder name. It then searches Google Drive for an existing folder with that name. If found, it prepares and uploads all files to that folder. If not found, it creates a new folder, then prepares and uploads the files into the newly created folder. Both paths ensure files retain their original names and are correctly placed.

## Output Details
The workflow uploads all submitted files to the specified (or newly created) Google Drive folder and completes silently upon success.

## Tags
google drive, file upload, form automation, folder management, batch processing
