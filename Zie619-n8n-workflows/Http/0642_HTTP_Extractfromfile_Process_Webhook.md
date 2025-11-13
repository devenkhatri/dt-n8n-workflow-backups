# Workflow Analysis for CV Screening with OpenAI

## Description
This workflow automates the screening of job candidates by downloading their CVs, extracting text content, and analyzing suitability against a job description using OpenAI’s AI model. It returns a structured evaluation including a matching score, strengths, and weaknesses.

## Input Details
The workflow is manually triggered and uses a predefined CV URL and job description stored as variables within the workflow.

## Process Summary
The workflow starts with a manual trigger, then sets key variables including the CV URL, job description, analysis prompt, and JSON schema. It downloads the CV file from the provided URL, extracts text from the PDF, and sends the extracted text along with the job description to OpenAI’s API for analysis using a structured prompt and JSON schema. The AI’s response is then parsed into a usable JSON object for further processing or storage.

## Output Details
The workflow outputs a parsed JSON object containing the candidate evaluation, including a matching percentage, summary, and structured reasons for suitability or unsuitability, which can be stored or used in downstream applications like Supabase.

## Tags
CV screening, OpenAI, PDF extraction, recruitment automation, AI analysis, n8n workflow, manual trigger, JSON parsing
