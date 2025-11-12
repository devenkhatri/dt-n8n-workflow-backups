# Workflow Analysis for HR Job Posting and Evaluation with AI

## Description
This workflow automates the end-to-end hiring process for an Automation Specialist role by collecting job applications, storing candidate data, using AI to evaluate resumes against the job description, shortlisting qualified candidates, generating personalized interview questionnaires, scheduling interviews, and preparing customized screening questions for phone interviews—all while updating an Airtable applicant tracker in real time.

## Input Details
The workflow is triggered by a form submission containing the candidate's name, email, phone, years of experience, and a PDF CV.

## Process Summary
When a candidate submits the job application form, their CV is uploaded to Google Drive and their details are saved to an Airtable 'Applicants' table. The CV is then downloaded, parsed for text, and sent to an AI model along with the job description (retrieved from Airtable) to generate a compatibility score. If the score is 0.7 or higher, the candidate is marked as 'Interviewing' in Airtable and proceeds; otherwise, they are marked as 'No hire'. Shortlisted candidates are presented with AI-generated interview questions via a form, and their responses are saved back to Airtable. A personalized email is then generated and sent to the candidate to schedule a phone interview. The workflow books a meeting using Google Calendar and logs the interview time in Airtable. Finally, it generates tailored screening questions for the interviewer based on the candidate’s CV and responses.

## Output Details
The workflow updates the Airtable 'Applicants' table with candidate details, AI-generated scores and notes, questionnaire responses, scheduled interview times, and tailored phone interview screening questions, and sends a personalized email to shortlisted candidates to schedule a phone interview.

## Tags
HR automation, AI recruitment, resume screening, Airtable integration, Google Drive, Google Calendar, OpenAI, form automation, candidate evaluation, interview scheduling
