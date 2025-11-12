# Workflow Analysis for AI CV Screening Workflow

## Description
This workflow automates the initial screening of job applicants for a Software Engineer position by using AI to analyze and rate CVs, while also managing communication and record-keeping.

## Input Details
The workflow is triggered by a form submission that collects the applicant's full name, email, salary expectation, LinkedIn profile, and a PDF resume.

## Process Summary
When a candidate submits an application form, the workflow extracts text from the uploaded PDF resume. This text is then analyzed by an AI model (Google Gemini) to generate a compatibility rating and hiring recommendation based on a predefined job description. The AI's evaluation, along with the candidate's details, is saved to a Google Sheet for tracking. Simultaneously, an automated confirmation email is sent to the candidate, and a detailed notification with the AI rating is sent to the HR team.

## Output Details
The workflow outputs an AI-generated compatibility rating stored in a Google Sheet, sends a confirmation email to the applicant, and notifies HR via email with the candidate's details and AI rating.

## Tags
AI, CV screening, recruitment automation, Google Sheets, Gmail, Google Gemini, form processing, HR automation
