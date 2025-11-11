# Workflow Analysis for MITRE ATT&CK-Powered Cybersecurity Analysis for Zendesk Tickets

## Description
This workflow enriches Zendesk support tickets with contextual cybersecurity intelligence by analyzing ticket content against the MITRE ATT&CK framework. It identifies relevant adversary Tactics, Techniques, and Procedures (TTPs), provides actionable remediation steps, and updates each ticket with structured threat intelligence.

## Input Details
The workflow is triggered manually or by new/updated Zendesk tickets, receiving ticket data including subject and description for analysis.

## Process Summary
First, the workflow retrieves all Zendesk tickets and processes them one by one. For each ticket, it uses an AI agent powered by GPT-4o to analyze the ticket content, leveraging a Qdrant vector store pre-loaded with MITRE ATT&CK data to identify relevant TTPs. The AI generates a structured response including alert summaries, remediation steps, historical patterns, and external references. This structured output is then used to update the original Zendesk ticket with MITRE technique IDs, tactics, and a detailed internal note summarizing the analysis.

## Output Details
The workflow updates each Zendesk ticket with MITRE ATT&CK technique ID, tactic name, and a comprehensive internal note containing cybersecurity analysis and remediation guidance.

## Tags
cybersecurity, MITRE ATT&CK, Zendesk, AI agent, vector store, Qdrant, threat intelligence, incident response, SIEM, LLM
