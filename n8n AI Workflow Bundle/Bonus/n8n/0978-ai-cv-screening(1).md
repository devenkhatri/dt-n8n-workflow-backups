# Workflow Analysis for AI CV Screening and Candidate Qualification

## Description
This workflow automates the screening of job applicant CVs using AI, qualifies candidates based on predefined criteria, and sends notifications for qualified applicants.

## Input Details
The workflow is manually triggered and receives applicant data including name, email, and CV link from a Google Sheet.

## Process Summary
The workflow first retrieves applicant data from a Google Sheet. It then downloads the CV from the provided link and extracts the text content. Next, it uses OpenAI to analyze the CV text against a job description, qualifies the candidate based on the analysis, and determines if the candidate is qualified. Finally, an email notification is sent for qualified candidates.

## Output Details
The workflow sends an email notification to a specified recipient when a candidate is qualified and updates the Google Sheet with the screening status and AI feedback.
