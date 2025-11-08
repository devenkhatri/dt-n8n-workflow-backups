# Workflow Analysis for Automated RFP Response Generator with AI

## Description
This workflow automates the process of responding to Request for Proposal (RFP) documents. It leverages Artificial Intelligence to extract questions from the RFP, generate contextual answers, compile them into a Google Document, and notify stakeholders upon completion.

## Input Details
The workflow is triggered by a webhook that receives an RFP document (PDF) and associated metadata such as title, ID, and a reply-to email address.

## Process Summary
First, the workflow extracts text from the submitted RFP document and sets variables for the response document. It then creates a new Google Document in Google Docs to serve as the RFP response draft, including initial metadata. Subsequently, an AI model identifies and extracts all questions from the RFP document. For each extracted question, an OpenAI Assistant generates a detailed answer using pre-configured company context. Finally, each question-answer pair is recorded into the Google Docs response document.

## Output Details
The workflow produces a Google Document containing the RFP questions and their AI-generated answers, and sends completion notifications via email and Slack.
