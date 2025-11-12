# Workflow Analysis for HR Job Posting and Evaluation with AI

## Description
This workflow automates the end-to-end hiring process for an Automation Specialist role by collecting applicant details via a form, storing resumes in Google Drive, saving applicant data in Airtable, using AI to score candidates based on job description and CV, shortlisting qualified candidates, generating personalized interview questionnaires, emailing shortlisted candidates, scheduling phone interviews, and preparing customized screening questions for the interview.

## Input Details
The workflow is triggered when a candidate submits a job application form containing personal details, years of experience, and a PDF CV.

## Process Summary
Upon form submission, the candidate's CV is uploaded to Google Drive and their details are saved to an Airtable 'Applicants' table. The CV is then downloaded and extracted as text, which is sent to an AI model along with the job description from Airtable to generate a qualification score. Candidates scoring 0.7 or above are marked as 'Interviewing' and receive a personalized email; others are marked as 'No hire'. For shortlisted candidates, AI-generated interview questionnaires are presented via a form, responses are saved back to Airtable, a meeting is scheduled via Google Calendar, and custom screening questions are generated and stored for the interviewer.

## Output Details
The workflow updates Airtable with candidate status, scores, questionnaire responses, interview times, and screening questions, and sends a personalized email to shortlisted candidates with a meeting invitation.

## Tags
HR automation, AI recruitment, candidate screening, Airtable integration, Google Drive, Google Calendar, OpenAI, form processing, interview scheduling, workflow automation
