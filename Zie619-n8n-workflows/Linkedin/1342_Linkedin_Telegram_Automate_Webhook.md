# Workflow Analysis for ✨🩷Automated Social Media Content Publishing Factory + System Prompt Composition

## Description
This n8n workflow automates the entire social media content publishing process, from dynamic content generation using AI and external prompts to multi-platform posting and archiving. It ensures brand consistency and efficiency across various social media channels.

## Input Details
The workflow is triggered either by a chat message providing a `chatInput` or by being executed from another workflow, receiving a `user_prompt` and a `route` (target social media platform).

## Process Summary
The workflow initiates upon receiving a chat message or being called by another workflow, extracting user prompt and target social media platform. It fetches and parses social media schema and system prompts from Google Docs, dynamically composing them for the AI content creator. An AI model (gpt-4o-mini) with web search capabilities generates platform-optimized social media content based on the composed prompts and schema. Concurrently, an image is generated via an external service (pollinations.ai), uploaded to imgbb.com, and saved to Google Drive. The generated content and image are sent for human approval via Gmail; if approved, the content is then published to the specified social media platform (X, Instagram, Facebook, LinkedIn, Threads, YouTube Shorts) and archived to Google Drive, with optional Telegram notifications.

## Output Details
The workflow publishes tailored social media posts (including images) to X-Twitter, Instagram, Facebook, LinkedIn, Threads, and YouTube Shorts, sends approval requests and status updates via Gmail and Telegram, and archives all post data and images to Google Drive.

## Tags
automation, n8n, production-ready, excellent, optimized
