# Workflow Analysis for AI-Powered Fastmail Draft Reply Generator

## Description
This workflow automatically monitors your IMAP inbox for new emails, uses OpenAI's GPT-4 to generate a casual and context-aware draft reply, and then saves this draft in your Fastmail drafts folder for review.

## Input Details
The workflow is triggered by an IMAP email account, which monitors for new, unread emails and receives their content and metadata.

## Process Summary
The workflow first fetches new unread emails from an IMAP account and extracts key fields like sender, subject, and body. It then sends this email content to OpenAI's GPT-4 to generate a casual draft response. Concurrently, it establishes a session with Fastmail, retrieves all mailbox IDs, and filters to find the drafts folder. Finally, it compiles the generated response, original email details, and Fastmail draft folder ID, and creates a new draft email in the user's Fastmail account.

## Output Details
The workflow generates a new draft email in the user's Fastmail "Drafts" folder, containing an AI-generated reply based on the incoming email.
