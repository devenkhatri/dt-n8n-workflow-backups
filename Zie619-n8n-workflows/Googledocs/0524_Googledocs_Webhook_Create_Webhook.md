# Workflow Analysis for AutoRFP: AI-Powered RFP Question Extraction and Response Generator

## Description
This workflow automates the process of responding to Requests for Proposals (RFPs) by using AI to extract questions from an uploaded RFP document, generating tailored answers using company-specific context, and compiling responses into a new Google Doc. Upon completion, it notifies the requester via email and the team via Slack.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint containing an RFP document (PDF), a title, a unique ID, and a reply-to email address.

## Process Summary
First, the workflow receives the RFP document and metadata via a webhook. It then extracts text from the PDF and creates a new Google Doc to store responses, adding metadata like title and requester. Next, it uses an AI model to identify and extract all questions from the RFP. The workflow loops through each question, using an OpenAI Assistant (preloaded with company information) to generate context-aware answers. Each question-answer pair is appended to the Google Doc.

## Output Details
The workflow produces a completed Google Doc with all RFP questions and AI-generated answers, and sends a completion notification via Gmail to the requester and via Slack to a designated channel.

## Tags
RFP, AI, OpenAI, Google Docs, automation, document processing, question answering, webhook, Slack, Gmail, LLM, sales enablement
