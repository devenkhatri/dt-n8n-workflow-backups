# Workflow Analysis for DSP Certificate w/ Google Forms

## Description
This workflow automatically generates and emails digital certificates to users who pass a quiz created via Google Forms. It monitors form responses in a Google Sheet, checks if the respondent's score meets the passing criteria, creates a personalized certificate using a Google Slides template, converts it to PDF, and sends it to the respondent's email.

## Input Details
The workflow is triggered when a new row (form response) is added to a specified Google Sheet linked to a Google Form, receiving respondent name, email, and quiz score.

## Process Summary
The workflow starts by monitoring a Google Sheet for new form responses. It extracts the respondent's name, email, and score. An 'If' condition checks whether the score is greater than the passing threshold (currently set to 3). If the score passes, the workflow copies a Google Slides certificate template, replaces the placeholder '[ NAME ]' with the respondent's actual name, converts the slide to a PDF, and emails the PDF certificate to the respondent.

## Output Details
The workflow produces a personalized PDF certificate and sends it as an email attachment to the respondent's email address if they pass the quiz.

## Tags
google forms, certificate generation, google sheets, google slides, automation, pdf conversion, email notification, quiz grading, n8n, production-ready
