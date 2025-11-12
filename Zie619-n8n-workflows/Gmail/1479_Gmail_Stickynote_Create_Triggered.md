# Workflow Analysis for Gmail AI auto-responder: create draft replies to incoming emails

## Description
This workflow automatically checks incoming Gmail messages, uses AI to determine if a reply is needed, and if so, generates a professional draft reply that appears in the same email thread.

## Input Details
The workflow is triggered by new incoming emails in a Gmail inbox (excluding emails sent by the user) via a polling Gmail trigger that checks every minute.

## Process Summary
The workflow starts by monitoring the Gmail inbox for new messages. For each incoming email, it uses an OpenAI model to assess whether the message requires a reply, returning a boolean in JSON format. If a reply is needed, a second OpenAI model generates a professional draft response based on the email content, following specific formatting and tone guidelines. The draft reply is then created in Gmail as part of the original conversation thread, with the subject prefixed with 'Re:' and the sender auto-filled. Errors during execution are captured and handled by a dedicated error node.

## Output Details
The workflow creates a Gmail draft reply in the same thread as the incoming email, ready for the user to review and send.

## Tags
Gmail, AI, auto-responder, email automation, OpenAI, draft reply, n8n, production-ready
