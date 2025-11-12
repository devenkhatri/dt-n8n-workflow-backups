# Workflow Analysis for AI-Powered File Organizer with Local File Trigger

## Description
This workflow automatically monitors a specified folder for new files and uses Mistral AI to intelligently organize them into appropriate subfolders. If suitable folders don't exist, the AI suggests new ones to create. The system then safely moves the files while avoiding overwrites by renaming duplicates with a random suffix.

## Input Details
The workflow is triggered automatically whenever a new file is added to the monitored local directory '/home/node/host_mount/shared_drive'.

## Process Summary
The workflow starts by detecting new files in a designated folder. It then lists all current files and subdirectories in that folder. Using this information, it sends a prompt to Mistral AI asking for suggestions on how to categorize and group the files into folders. The AI's structured response is parsed into folder-file mappings. Finally, the workflow executes shell commands to create any missing folders and move the files accordingly, renaming duplicates if necessary.

## Output Details
The workflow reorganizes files in the monitored directory by moving them into AI-suggested subdirectories, creating new folders as needed and handling file name conflicts by renaming duplicates.

## Tags
file organization, AI automation, local file trigger, Mistral AI, folder management, n8n workflow, production-ready, automation
