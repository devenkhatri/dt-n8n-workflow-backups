# Workflow Analysis for CV Screening with OpenAI

## Description
This workflow automates the screening of candidate resumes by extracting text from a CV PDF, analyzing it against a job description using OpenAI's GPT model, and returning a structured evaluation including a match percentage, summary, and suitability insights.

## Input Details
The workflow is manually triggered and receives a direct URL to a candidate's CV (PDF) and a job description via preset variables in the 'Set Variables' node.

## Process Summary
The workflow starts by setting variables including the CV file URL and job description. It downloads the CV from the provided URL, then extracts text from the PDF. This extracted text is sent to OpenAI's API along with a system prompt and JSON schema to enforce structured output. OpenAI analyzes the candidate's suitability for the job and returns a formatted response, which is then parsed into a JSON object for downstream use.

## Output Details
The workflow outputs a structured JSON object containing the candidate match percentage, summary, and detailed reasons for suitability or unsuitability, ready for storage or further processing.

## Tags
recruitment, CV screening, OpenAI, PDF extraction, HR automation, resume analysis, AI evaluation
