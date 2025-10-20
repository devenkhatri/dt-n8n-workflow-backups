# Workflow Analysis for ERPNext Candidate Automation

## Description
This workflow automates the candidate application process in ERPNext, creating a job applicant, scheduling an interview, and updating the applicant status.

## Input Details
This workflow is triggered manually.

## Process Summary
First, the workflow gets system settings from ERPNext for candidate tagging and interview templates. It then creates a new job applicant in ERPNext with provided candidate details and contact information. Next, it schedules an interview for the newly created applicant. Finally, the workflow updates the job applicant's status to "Interview Scheduled" in ERPNext.

## Output Details
The workflow updates the job applicant in ERPNext with "Interview Scheduled" status.
