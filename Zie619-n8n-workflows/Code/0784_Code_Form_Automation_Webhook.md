# Workflow Analysis for Formtrigger Workflow

## Description
This workflow automatically captures form submissions and uses the data to personalize a Google Doc template by replacing placeholders (like {{name}}) with actual form responses. It copies a template document from Google Drive and updates it with the submitted information via the Google Docs API.

## Input Details
The workflow is triggered by a web form submission that includes at least a required 'name' field, and potentially other fields that correspond to placeholders in a Google Doc template.

## Process Summary
The workflow starts when a user submits a form. It then copies a specified Google Doc template from Google Drive. Next, it formats the form data into key-value pairs and transforms them into a structure compatible with the Google Docs API's replaceAllText request. Finally, it sends an authenticated HTTP request to the Google Docs API to replace all matching placeholders in the copied document with the actual form data.

## Output Details
The workflow produces a personalized copy of a Google Doc with form data inserted in place of template placeholders, stored in the user's Google Drive.

## Tags
form automation, Google Docs, Google Drive, document generation, template replacement, n8n workflow
