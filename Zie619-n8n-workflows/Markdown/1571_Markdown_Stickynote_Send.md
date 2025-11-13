# Workflow Analysis for Very simple Human in the loop system email with AI e IMAP

## Description
This workflow automates the handling of incoming emails, summarizes their content, generates appropriate responses, and validates them through a "Human in the loop" system before sending the final reply.

## Input Details
The workflow is triggered by new incoming emails received via an IMAP email account.

## Process Summary
First, the workflow reads an incoming email and converts its HTML content to Markdown format. Next, an AI model summarizes the email content to extract key information. Subsequently, another AI agent drafts a professional reply based on the summarized email and system messages. This drafted email, along with the original message, is then sent for human approval. If the human approves the AI-generated reply, the workflow proceeds to send the final email.

## Output Details
The workflow sends an email for human approval and, upon approval, sends an AI-generated reply to the original sender of the email.

## Tags
automation,n8n,production-ready,excellent,optimized,email,ai,imap,human-in-the-loop,summarization
