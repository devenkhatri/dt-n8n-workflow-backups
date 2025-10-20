# Workflow Analysis for AI-Powered CV Evaluation for HR

## Description
This workflow automates the process of evaluating resumes (CVs) for HR professionals using AI. It extracts relevant information from CVs, ranks candidates based on predefined criteria, and provides a summary for efficient candidate screening.

## Input Details
The workflow is manually triggered and receives a list of CV filenames as input.

## Process Summary
The workflow iterates through each provided CV filename. For each CV, it loads the file content and sends it to an AI model along with job description details for evaluation. The AI model extracts key information and provides a compatibility score. Finally, the workflow reformats the AI response into a structured output for each candidate.

## Output Details
The workflow outputs a summary of each evaluated CV, including a compatibility score, key extracted information, and a summary of the candidate, in a structured JSON format.
