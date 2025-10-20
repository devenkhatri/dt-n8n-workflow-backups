# Workflow Analysis for AI CV Screening and Candidate Profile Generation

## Description
This workflow automates the screening of CVs using AI, extracts key information, and generates a structured candidate profile and an executive summary for recruitment purposes. It also allows for manual review and updates of the candidate data.

## Input Details
The workflow is triggered manually and requires a PDF file (CV) and a prompt containing the job description as input.

## Process Summary
The workflow first reads the PDF CV and then uses an AI model to extract specified information such as the candidate's name, contact details, experience, and educational background based on a job description. It generates a comprehensive candidate profile in JSON format and an executive summary. The AI also assigns a fit score and provides comments. Finally, the workflow presents the extracted data in a Human-in-the-Loop node for review and potential updates before generating the final JSON output.

## Output Details
The workflow outputs a JSON object containing the candidate's detailed profile, an executive summary, and an AI-generated fit score and comments.
