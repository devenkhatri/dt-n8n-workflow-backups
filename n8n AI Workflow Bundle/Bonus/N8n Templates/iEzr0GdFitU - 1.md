# Workflow Analysis for Automated AI Email Responder and Manager

## Description
This workflow automatically listens for new incoming emails in a Gmail account and uses a large language model (like OpenAI's GPT) to analyze the email's content, draft a professional, context-aware reply, and send it back to the original sender, significantly reducing manual inbox management.

## Input Details
The workflow is triggered by the arrival of a new, unread email in a specified Gmail inbox.

## Process Summary
When a new email arrives, the workflow extracts its content and passes it to the OpenAI node, along with a system prompt to draft a professional response. The AI model generates the reply text, which is then captured and prepared by a subsequent Set node. Finally, the prepared response is sent back to the original sender using the Gmail node, with the original subject line appropriately prefixed.

## Output Details
The workflow sends an automatically generated email response back to the sender of the triggering email via the Gmail node.
