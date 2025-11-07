# Workflow Analysis for AI-Powered Job Application with CV Processing and Airtable Integration

## Description
This n8n workflow automates a two-step job application process, starting with a form for CV submission. It uses AI to classify the uploaded document as a CV, extract relevant applicant information, and pre-fill a second application form, finally storing all data and the CV in Airtable.

## Input Details
The workflow is triggered by an applicant submitting their name and a PDF CV through a two-step web form.

## Process Summary
First, the workflow extracts text from the uploaded PDF CV and uses an AI model to classify if it is indeed a CV; if not, the applicant is prompted to re-upload. If valid, another AI model extracts specific candidate details like name, address, email, education, and skills, based on a provided job description. This extracted data, along with the original CV, is then saved into an Airtable database. Finally, the applicant is redirected to a second form, pre-filled with the extracted information, which they can review and submit to update their Airtable record.

## Output Details
The workflow saves the applicant's extracted information and their original PDF CV into an Airtable database, and provides a multi-step form experience for the applicant.
