# Workflow Analysis for Resume Data Extraction and PDF Generation with Gotenberg

## Description
This workflow extracts specified data from a resume file that is provided in a webhook and then uses Gotenberg to generate a PDF document containing the extracted information.

## Input Details
The workflow is triggered by an HTTP webhook that receives a file and parameters containing instructions on which data to extract from the resume.

## Process Summary
First, the workflow receives a file and custom data fields via a webhook. Next, it uses a custom Python script to extract the requested fields from the uploaded resume. Then it constructs an HTML document using the extracted data to format the content for the final PDF. Finally, it converts the HTML content into a PDF document using the Gotenberg service.

## Output Details
The workflow outputs a PDF file containing the extracted resume information to the response of the triggering webhook.
