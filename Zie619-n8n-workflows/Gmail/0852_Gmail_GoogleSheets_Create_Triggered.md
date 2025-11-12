# Workflow Analysis for Resume Screener from Gmail to Sheets

## Description
This workflow automatically screens job applicant resumes received via Gmail, extracts key details like name, email, LinkedIn, and a suitability score using AI, then logs this information into a Google Sheet for review.

## Input Details
The workflow is triggered when a new unread email with an attachment arrives in a Gmail inbox.

## Process Summary
The workflow starts by monitoring Gmail for new unread emails with attachments. When detected, it downloads the attached PDF resume and extracts its text content. This text is sent to an OpenAI GPT-4o-mini model with instructions to analyze the resume and extract structured data: name, email, LinkedIn URL, and a score. The structured output is then formatted according to a predefined schema and appended as a new row in a specified Google Sheet along with the full resume text.

## Output Details
The workflow adds a new row to a Google Sheet containing the candidate’s name, email, LinkedIn profile, resume score, and full extracted resume text.

## Tags
resume screening, Gmail automation, Google Sheets, OpenAI, PDF text extraction, AI agent, recruitment automation, structured output
