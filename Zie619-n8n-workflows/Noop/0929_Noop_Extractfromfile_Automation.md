# Workflow Analysis for OpenAI e-mail classification - application

## Description
Automated workflow: OpenAI e-mail classification - application. This workflow integrates 8 different services: textClassifier, stickyNote, informationExtractor, stopAndError, lmChatOpenAi. It contains 14 nodes and follows best practices for error handling and security.

## Input Details
The workflow is triggered by an email received through an IMAP account and processes the email's content and attachments.

## Process Summary
The workflow automatically retrieves new emails from a configured IMAP account. It extracts text content from both the email body and any attached PDF files. Using the combined text, the email is classified into predefined categories such as "job_application," "inbound_lead," or "invoice." If an email is classified as a "job_application," the workflow proceeds to extract specific applicant details like name, age, residence, study, and work experience. This classified and extracted data is then prepared for further automated actions, potentially involving OpenAI for deeper analysis or routing to specialized sub-workflows.

## Output Details
The workflow produces classified email data and extracted key information from job applications, making it ready for downstream automated processing or routing to specific workflows based on the email category.

## Tags
automation,n8n,production-ready,excellent,optimized
