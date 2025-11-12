# Workflow Analysis for Automated Resume Review System Using OpenAI + Google Sheets

## Description
This workflow automates the resume review process by collecting candidate information through a form, extracting key details from their uploaded resume using AI, summarizing their qualifications, and having an AI-powered HR expert evaluate their fit for a specified role. The results—including candidate details, AI-generated summary, and hiring recommendation—are saved to a Google Sheet for tracking.

## Input Details
The workflow is triggered when a candidate submits a form containing their first name, last name, email, and a PDF resume.

## Process Summary
Upon form submission, the resume is uploaded to Google Drive and its text is extracted. Two parallel extraction steps gather personal information (name, email, city, etc.) and professional qualifications (education, job history, skills). The extracted data is merged and used to generate a concise professional summary. An AI HR expert then evaluates the candidate against a predefined job profile, assigning a 1–10 rating and providing reasoning. Finally, all data—including the rating and consideration notes—is appended to a Google Sheet.

## Output Details
The workflow appends a structured record of the candidate’s information, AI-generated summary, HR rating (1–10), and hiring consideration notes to a Google Sheet named 'HR New'.

## Tags
resume review, AI hiring, OpenAI, Google Sheets, Google Drive, form automation, candidate screening, n8n, HR automation, PDF extraction
