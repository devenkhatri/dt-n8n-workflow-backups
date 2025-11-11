# Workflow Analysis for CallForge - AI Sales Call Analyzer

## Description
This workflow automatically analyzes sales call transcripts to extract actionable insights for sales, marketing, and product teams. It identifies use cases, objections, pain points, competitor mentions, integration needs, and more, then routes structured data to respective departmental workflows.

## Input Details
The workflow is triggered manually or via another workflow and receives sales call transcript data along with contextual metadata such as attendee names, company info, competitors, and integrations.

## Process Summary
The workflow first standardizes the transcript and context into a unified prompt. It then runs three parallel AI analyses: one for sales insights (use cases, objections, budget, timeline, etc.), one for marketing insights (landing page opportunities, content requests, recurring topics), and one for product feedback (sentiment, feature gaps, AI/ML usage). Each AI response is parsed into structured JSON. The parsed data is enriched with original metadata and sent to dedicated sub-workflows for sales, marketing, and product teams. Finally, all processed data is merged and a success status is generated.

## Output Details
The workflow outputs structured insights to three downstream sub-workflows (Sales AI Data Processor, Marketing AI Data Processor, and Product AI Data Processor), which typically feed into Notion or Salesforce, and returns a success confirmation message.

## Tags
sales automation, AI analysis, call transcription, Gong integration, marketing insights, product feedback, n8n workflow, structured data extraction, CRM enrichment, Notion integration
