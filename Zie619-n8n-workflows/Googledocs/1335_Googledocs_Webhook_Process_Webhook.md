# Workflow Analysis for AutoRFP Response Generator

## Description
This workflow automates the process of responding to Request for Proposal (RFP) documents by extracting questions from an uploaded RFP PDF, using AI to generate informed answers based on company knowledge, and compiling the responses into a new Google Doc. Once complete, it notifies the requester via email and the team via Slack.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint containing an RFP document (PDF), a title, an ID, and a reply-to email address.

## Process Summary
The workflow starts by receiving an RFP document and metadata via a webhook. It extracts text from the PDF, creates a new Google Doc for the response, and adds metadata to it. Using an LLM, it identifies and lists all questions from the RFP. It then loops through each question, uses an OpenAI Assistant (preloaded with company documents) to generate answers, and appends each Q&A pair to the Google Doc. Finally, it sends an email to the requester and a Slack message to the team.

## Output Details
The workflow produces a Google Doc containing extracted RFP questions and AI-generated answers, and sends completion notifications via Gmail and Slack.

## Tags
RFP, AI, automation, Google Docs, OpenAI, webhook, document processing, sales, proposal response, n8n
