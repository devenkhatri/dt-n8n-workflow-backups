# Workflow Analysis for AI Agent - Cv Resume - Automated Screening, Sorting, Rating and Tracker System

## Description
This workflow automatically screens, sorts, rates, and tracks job candidates' resumes using AI. It compares each resume against a job description, categorizes candidates as Rejected, Keep-in-View (KIV), or Shortlisted, moves their files into appropriate folders, updates a Google Sheet tracker with AI-generated scores and reasons, and sends email notifications with the decision.

## Input Details
The workflow is triggered when a new PDF resume file is added to a specific 'Unfiltered' Google Drive folder, and it fetches the current job description from a Google Doc.

## Process Summary
1. When a new resume is added to the 'Unfiltered' folder in Google Drive, the workflow triggers. 2. It downloads the resume file and extracts text from it (assuming PDF format). 3. It retrieves the job description from a predefined Google Doc. 4. An AI agent (using Groq's Llama 4 model) compares the candidate’s profile with the job description and decides whether to Reject, KIV, or Shortlist the candidate, along with a reason and score. 5. Based on the AI decision, the workflow moves the resume to the corresponding folder, updates a Google Sheet tracker with the candidate’s details and AI evaluation, and sends an email notification.

## Output Details
The workflow updates a Google Sheet tracker with the candidate’s name, AI verdict, score, and reason; moves the resume file to a categorized Google Drive folder (Rejected/KIV/Shortlisted); and sends an email notification with the decision details.

## Tags
AI, resume screening, automation, Google Drive, Google Sheets, Gmail, Groq, Llama 4, hiring, recruitment, CV analysis, n8n
