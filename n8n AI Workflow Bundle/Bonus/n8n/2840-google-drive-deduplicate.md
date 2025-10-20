# Workflow Analysis for Google Drive Deduplication on Schedule

## Description
This workflow automates the process of identifying and moving duplicate files in a specified Google Drive folder to a trash folder, helping to maintain an organized and clutter-free cloud storage.

## Input Details
The workflow is triggered manually or on a schedule, allowing for periodic checks of your Google Drive.

## Process Summary
The workflow starts by listing all files in a designated Google Drive folder. It then iterates through these files, creating a list of filenames without extensions. After sorting and identifying duplicate filenames, it proceeds to move all but the oldest version of each duplicate file to the Google Drive trash.

## Output Details
The workflow moves identified duplicate files (excluding the oldest) to the Google Drive trash, cleaning up the specified folder.
