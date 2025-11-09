# Workflow Analysis for The Recap AI - Marketing Team Agent

## Description
An AI-powered marketing assistant that helps The Recap AI marketing team create and repurpose content across multiple channels—including newsletters, social media posts, short-form video scripts, and research reports—while maintaining brand consistency and leveraging daily memory for context-aware content generation.

## Input Details
The workflow is triggered either by a webhook request or an incoming chat message containing a user's content request or instruction.

## Process Summary
The agent uses Google's Gemini 2.5 Pro model with a daily memory context window to understand and respond to user requests. Based on the request, it can generate a newsletter, create images, repurpose newsletter content into Twitter threads, write short-form video scripts, or perform deep research on AI-related topics using Perplexity. It can also generate talking head videos from scripts and email detailed research reports to specified recipients.

## Output Details
The workflow produces marketing content such as newsletters, social media threads, video scripts, custom images, research reports, and avatar videos, which are either returned to the user or sent via email depending on the tool used.

## Tags
AI Agent, Content Creation, Content Repurposing, Marketing Automation, Newsletter Generator, Social Media, Video Script, Research Report, Email Automation
