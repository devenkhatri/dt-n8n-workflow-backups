# Workflow Analysis for Credentials Transfer

## Description
This workflow allows users to securely copy credentials from one n8n instance to another by selecting a source credential and a destination instance through guided forms.

## Input Details
The workflow is triggered by a form submission and receives user selections for the source credential and target n8n instance.

## Process Summary
The workflow begins by exporting all credentials from the current n8n instance using a CLI command and reads the output file. It converts the exported credentials into JSON format and dynamically generates dropdown options for both available credentials and pre-configured remote instances. The user is guided through two forms: one to select the destination instance and another to choose the credential to transfer. Based on these selections, the workflow prepares a request with the credential data and the appropriate API key, then sends it to the destination instance via an HTTP POST request.

## Output Details
The workflow displays a success or error message to the user via form completion pages, confirming whether the credential was successfully transferred to the selected instance.

## Tags
n8n, credentials, automation, data transfer, workflow, form, http request, security, production-ready
