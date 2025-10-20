# Workflow Analysis for ATS AI Assessment and Resume Parsing

## Description
This workflow automates the assessment of job applications using AI, parsing resumes and cover letters, and comparing them against job descriptions and ideal candidate profiles to provide a suitability score and detailed feedback.

## Input Details
The workflow is triggered by an HTTP POST request containing application data, including resume, cover letter, job description, and ideal candidate profile.

## Process Summary
First, the workflow extracts text from the uploaded resume and cover letter. Then, it uses AI to extract key entities from these documents. It subsequently compares the extracted information with the job description and ideal candidate profile using another AI model to calculate suitability scores. Finally, it uses AI to provide detailed feedback on the candidate's suitability.

## Output Details
The workflow returns a detailed JSON response containing the parsed resume information, suitability scores, and AI-generated feedback.
