# Workflow Analysis for AI CV Screening Workflow

## Description
This workflow automates the initial screening of job applicants for a Software Engineer position by collecting their application details and CV, using AI to analyze and rate the candidateâ€™s fit for the role, storing the information in a Google Sheet, and sending confirmation and notification emails to the applicant and HR team respectively.

## Input Details
The workflow is triggered by a web form submission that collects the applicantâ€™s full name, email, salary expectation, LinkedIn profile, and a PDF resume.

## Process Summary
The workflow starts when a candidate submits an application form with their details and CV. The PDF resume is extracted into text, then analyzed by an AI model (Google Gemini) that generates a compatibility rating and recommendation based on the job description for a Software Engineer role. The candidateâ€™s information along with the AI rating is saved to a Google Sheet. Finally, two emails are sent: one to the candidate confirming receipt of their application, and another to the HR team notifying them of the new CV and including the AI-generated insights.

## Output Details
The workflow outputs candidate data and AI analysis to a Google Sheet, sends a confirmation email to the applicant, and sends a notification email with AI insights to the HR team.

## Tags
AI recruitment, CV screening, Google Gemini, automated hiring, Gmail integration, Google Sheets, form automation, talent acquisition
