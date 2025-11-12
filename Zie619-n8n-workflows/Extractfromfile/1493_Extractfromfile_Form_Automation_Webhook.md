# Workflow Analysis for AI-Powered Job Application Processing Workflow

## Description
This workflow automates the job application process by accepting a CV upload, validating and extracting relevant information using AI, pre-filling an application form, and saving all data to an Airtable-based applicant tracking system.

## Input Details
The workflow is triggered by a web form where applicants submit their name, a PDF CV file, and agree to terms and conditions.

## Process Summary
The workflow begins by extracting text from the uploaded PDF CV. It then uses AI to classify the document as a valid CV and extracts structured applicant data (name, contact info, education, skills, experience, and a tailored cover letter) by comparing the CV against a specific job posting. This extracted data is saved to Airtable along with the original CV file. The applicant is then redirected to a second form, pre-filled with the extracted data, allowing them to review and edit before final submission, which updates their record in Airtable.

## Output Details
The workflow saves the applicant's structured data and original CV file to an Airtable base and displays a success message to the user after the final form submission.

## Tags
job application, AI, PDF extraction, form automation, Airtable, LLM, document classification, recruitment, n8n
