# Workflow Analysis for The Recap AI - Gmail Agent and Knowledge Base Builder

## Description
This workflow automates two key processes: first, it builds a comprehensive business knowledge base for a lawn care service company by scraping their website, processing the content with an AI, and storing it as a Google Doc; second, it acts as an intelligent Gmail agent that uses this knowledge base to analyze incoming emails, determine if a response is appropriate, generate helpful replies, and log all interactions.

## Input Details
The workflow is triggered either manually via a form submission providing a website URL and Google Drive folder ID, or automatically when a new email is received in Gmail.

## Process Summary
Upon manual trigger, the workflow scrapes all accessible URLs from a provided website. The scraped content is then processed by a large language model (LLM) to synthesize a structured business knowledge base, deduplicating information and organizing it into categories. This knowledge base is converted to HTML and uploaded as a new Google Document to a specified Google Drive folder. Separately, an intelligent AI agent continuously monitors incoming Gmail messages, analyzes their content, retrieves relevant information from the Google Docs knowledge base, and decides whether to compose and send an automated, professional email reply, logging the interaction and decision in a Google Sheet.

## Output Details
The workflow produces a structured business knowledge base as a Google Document in a designated Google Drive folder, and for incoming emails, it may send automated replies via Gmail and logs all agent activities to a Google Sheet.
