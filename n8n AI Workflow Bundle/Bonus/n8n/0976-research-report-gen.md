# Workflow Analysis for Automated Research Report Generator

## Description
This workflow automates the generation of research reports based on a user-provided topic. It leverages AI to gather information, structure the report, and format it into a professional document.

## Input Details
This workflow is triggered by an HTTP request containing the research topic and optionally, a directory ID for Google Drive.

## Process Summary
The workflow first constructs a prompt from the input topic. It then uses an AI model to generate a research report based on this prompt. The generated report is then converted into a Google Docs document. Finally, if a directory ID is provided, the Google Docs file is moved to the specified Google Drive folder, otherwise it remains in the root folder.

## Output Details
The workflow outputs a Google Docs research report, either in a specified Google Drive folder or the root folder.
