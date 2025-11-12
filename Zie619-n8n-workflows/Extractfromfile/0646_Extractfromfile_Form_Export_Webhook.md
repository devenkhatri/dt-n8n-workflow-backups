# Workflow Analysis for AI-Powered Job Application Processing Workflow

## Description
This workflow automates the job application process by allowing candidates to upload a CV, using AI to extract and validate relevant information, and then pre-filling a second application form to reduce duplicate data entry. The extracted data and original CV are saved to an Airtable-based applicant tracking system.

## Input Details
The workflow is triggered by a web form where applicants submit their name, a PDF CV, and acknowledge terms and conditions.

## Process Summary
First, the applicant uploads a CV via a form. The PDF is extracted and classified to confirm it's a valid resume. If valid, an AI model analyzes the CV in the context of a specific job posting to extract structured details like name, email, skills, and experience, and even generates a tailored cover letter. This structured data is saved to Airtable along with the original CV file. The applicant is then redirected to a second form, prefilled with the AI-extracted data, where they can review and edit before final submission. The final data is again saved to Airtable.

## Output Details
The workflow saves the applicant's structured information and CV file to an Airtable base and displays a success message to the applicant after final form submission.

## Tags
AI, job application, CV parsing, resume extraction, form automation, Airtable, OpenAI, document processing, applicant tracking, n8n
