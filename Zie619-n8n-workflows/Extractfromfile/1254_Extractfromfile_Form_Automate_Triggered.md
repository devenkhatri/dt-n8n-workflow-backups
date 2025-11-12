# Workflow Analysis for HR-focused automation pipeline with AI

## Description
This workflow automates the initial screening of job applicants by extracting key information from their submitted CVs, evaluating their fit against a desired job profile using AI, and logging the results in a Google Sheet for HR review.

## Input Details
The workflow is triggered when a candidate submits a form with their name, email, and a PDF CV.

## Process Summary
Upon form submission, the CV is uploaded to Google Drive and its text is extracted. Two parallel AI extraction steps pull out personal details (like city, birthdate, phone) and professional qualifications (education, job history, skills). These are merged and summarized into a concise candidate profile. The system then compares this profile against a predefined ideal candidate description using an AI-powered HR expert, which assigns a suitability score (1–10) and justification. Finally, all extracted data, summary, score, and considerations are saved to a Google Sheet.

## Output Details
The workflow outputs structured candidate data, a suitability score, and HR considerations into a Google Sheet named 'Ricerca WebDev'.

## Tags
HR automation, AI recruitment, CV parsing, Google Sheets integration, candidate screening, form automation, n8n workflow
