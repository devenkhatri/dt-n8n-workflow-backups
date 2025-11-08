# Workflow Analysis for AI-Powered MITRE ATT&CK Enrichment for Zendesk and Chat

## Description
This workflow enhances cybersecurity incident response by automatically enriching Zendesk tickets with MITRE ATT&CK intelligence and providing an interactive AI chat for analysis. It extracts TTPs, remediation steps, and historical context from security alerts, utilizing OpenAI and a Qdrant vector store.

## Input Details
The workflow is triggered either manually to embed MITRE ATT&CK data, by a scheduled retrieval of Zendesk tickets, or via a chat message for interactive AI-driven cybersecurity analysis.

## Process Summary
The workflow first allows for manual setup by extracting MITRE ATT&CK data from Google Drive, embedding it with OpenAI, and storing it in a Qdrant vector database. It then retrieves all Zendesk tickets and processes them individually. For each ticket, an AI agent, leveraging OpenAI's gpt-4o and the MITRE ATT&CK knowledge base in Qdrant, analyzes the alert's subject and description. The AI agent extracts TTP information, actionable remediation steps, historical context, and external resources, which are then structured and used to update the original Zendesk ticket with an internal note and custom fields. Additionally, the workflow offers an interactive chat interface where users can query a similar AI agent for real-time cybersecurity insights based on the MITRE ATT&CK framework, complete with conversational memory.

## Output Details
The workflow updates Zendesk tickets with comprehensive MITRE ATT&CK-based cybersecurity insights and provides real-time, expert responses to user queries via a chat interface.
