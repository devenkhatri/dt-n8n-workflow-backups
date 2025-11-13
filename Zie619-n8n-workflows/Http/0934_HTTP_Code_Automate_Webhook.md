# Workflow Analysis for Automated PDF to HTML Conversion

## Description
This workflow automatically converts newly uploaded PDF files from a specific Google Drive folder into HTML format and saves the converted HTML file back to Google Drive, eliminating manual intervention.

## Input Details
The workflow is triggered when a new file is created in a specified Google Drive folder, and it receives file metadata including the MIME type and web view link.

## Process Summary
The workflow starts by monitoring a Google Drive folder for new files. When a file is added, it checks if the file is a PDF using its MIME type. If it is a PDF, the workflow sends the file’s web view link to an external API via an authenticated HTTP POST request to convert it to HTML. The returned HTML content is then converted into a binary file using a code node. Finally, the HTML file is uploaded to a designated Google Drive folder.

## Output Details
The workflow produces an HTML file from the original PDF and saves it to a specified Google Drive folder.

## Tags
PDF conversion, HTML, Google Drive, automation, n8n, document processing, API integration, production-ready
