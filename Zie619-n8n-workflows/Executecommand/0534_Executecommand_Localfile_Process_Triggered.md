# Workflow Analysis for AI-Powered File Organizer with Local File Trigger

## Description
This workflow automatically monitors a specified folder for new files and uses Mistral AI to intelligently organize them into appropriate subfolders. If suitable folders don’t exist, the AI suggests new ones to create. The system then moves the files accordingly, helping maintain a clean and structured directory.

## Input Details
The workflow is triggered when new files are added to a specified local directory mounted in the n8n environment.

## Process Summary
The workflow starts by detecting new files in a monitored directory. It then lists all current files and folders in that directory. This list is sent to Mistral AI, which suggests logical groupings and target folders for each file. The AI's structured response is parsed into a list of file-to-folder mappings. Finally, the workflow executes shell commands to move each file into its suggested folder, creating new folders if needed and avoiding filename conflicts by appending random strings to duplicates.

## Output Details
The workflow reorganizes the file system by moving files into AI-suggested subdirectories, creating new folders as needed.

## Tags
file organization, AI automation, local file trigger, Mistral AI, folder management, n8n workflow, automated file sorting, execute command, production-ready
