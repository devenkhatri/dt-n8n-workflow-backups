# Workflow Analysis for Fastmail AI Email Reply Drafting

## Description
This workflow automatically drafts personalized email replies using OpenAI's GPT-4 and saves them to the Fastmail Drafts folder for user review before sending.

## Input Details
The workflow is triggered by new unread emails arriving in an IMAP inbox, from which it extracts sender, subject, body, and message metadata.

## Process Summary
When a new email arrives, the workflow extracts key email fields and sends them to OpenAI's GPT-4 to generate a contextual, casual reply. Concurrently, it connects to Fastmail's JMAP API to retrieve mailbox information and identify the Drafts folder ID. It then formats the AI-generated response into a proper email draft, preserving the original message's context and threading. Finally, the draft email is uploaded to the Fastmail Drafts folder via the JMAP API.

## Output Details
The workflow creates and uploads a draft reply email to the user's Fastmail Drafts folder, ready for review and manual sending.

## Tags
email automation, AI reply, Fastmail, OpenAI, JMAP API, IMAP, draft email
