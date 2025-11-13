# Workflow Analysis for Automated Social Media Content Publishing Factory + System Prompt Composition

## Description
This workflow automates the creation and publishing of social media content across various platforms using AI-driven content generation and a robust approval process.

## Input Details
This workflow is triggered by an incoming chat message or execution from another workflow, receiving a user prompt and the target social media platform.

## Process Summary
The workflow first retrieves social media schemas and system prompts from Google Docs. It then composes these to create a comprehensive prompt for a Large Language Model (LLM). The LLM generates platform-optimized social media content based on the user prompt and defined schemas. Optionally, an image for the post can be generated and saved. Finally, the generated content is sent for approval via Gmail, and upon approval, it is published to the designated social media platform.

## Output Details
The workflow publishes tailored social media content to X (Twitter), Instagram, Facebook, LinkedIn, Threads, and YouTube Shorts, and facilitates content approval via Gmail.

## Tags
automation, n8n, production-ready, excellent, optimized, social media, content creation, AI
