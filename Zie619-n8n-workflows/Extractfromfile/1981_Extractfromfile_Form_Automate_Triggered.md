# Workflow Analysis for HR-focused automation pipeline with AI

## Description
This workflow automates the initial screening of job applicants by extracting data from their CVs, summarizing their qualifications, and evaluating how well they match a desired job profile using AI. The results—including a score and HR considerations—are stored in a Google Sheet for review.

## Input Details
The workflow is triggered when a candidate submits a form with their name, email, and a PDF CV.

## Process Summary
First, the submitted CV is uploaded to Google Drive and its text is extracted. Then, two parallel AI extraction steps gather personal details (like phone, city, and birthdate) and professional qualifications (education, job history, and skills). These details are merged and summarized into a concise candidate profile. The system then compares this profile against a predefined job description using an AI-powered HR expert prompt to generate a suitability score (1-10) and written considerations. Finally, all data—including the score and summary—is saved to a Google Sheet.

## Output Details
The workflow stores structured candidate data, including personal info, qualifications, AI-generated summary, suitability score, and HR considerations, in a Google Sheet named 'Ricerca WebDev'.

## Tags
HR automation, AI recruitment, CV parsing, candidate screening, Google Sheets integration, Google Drive, AI evaluation, form automation, n8n workflow, production-ready
