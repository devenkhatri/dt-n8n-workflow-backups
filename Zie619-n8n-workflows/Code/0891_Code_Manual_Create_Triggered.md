# Workflow Analysis for Create Google Drive Folders by Path

## Description
This workflow automatically creates a nested folder structure in Google Drive based on a provided path string (e.g., 'Projects/Clients/Reports') and returns the ID of the final folder for immediate use.

## Input Details
The workflow is triggered manually or by another workflow and receives two input parameters: 'google_drive_folder_id' (ID of the parent folder or 'root') and 'desired_path' (a slash-separated folder path string).

## Process Summary
The workflow first splits the desired path into individual folder names. It then enters a loop where it checks if the next folder in the path exists within the current parent folder in Google Drive. If the folder doesn't exist, it creates it. After handling the current folder, it shifts to the next folder in the path and repeats the process using a recursive workflow execution pattern until all folders are created. Finally, it returns the Google Drive ID of the last (deepest) folder in the path.

## Output Details
The workflow outputs the Google Drive folder ID of the last folder in the created path, which can be used by the calling workflow to upload files or perform further actions.

## Tags
Google Drive, folder creation, nested folders, path parsing, recursive workflow, automation, n8n, production-ready
