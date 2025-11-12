# Workflow Analysis for 🤓 Conversion Rate Optimizer

## Description
This workflow helps business owners and marketers improve their website's conversion rate by analyzing their landing page content and providing a fun, personalized critique along with 10 actionable, cutting-edge optimization ideas.

## Input Details
The workflow is triggered by a form submission where the user provides a URL to their landing page.

## Process Summary
The workflow starts by collecting a landing page URL via a form. It then scrapes the content of the provided URL using an HTTP request. The scraped content is passed to an AI prompt that instructs an expert-level Conversion Rate Optimization (CRO) persona to roast the landing page and generate 10 specific, creative, and personalized CRO recommendations. The prompt is designed to ensure the AI output is engaging, unconventional, and tailored to the actual content of the landing page. The workflow appears to use an OpenAI model (likely o1) with high reasoning effort to generate the response.

## Output Details
The workflow produces a detailed AI-generated roast and 10 targeted CRO recommendations, though the final delivery method (e.g., email, UI display) is not explicitly defined in the provided nodes.

## Tags
conversion rate optimization, CRO, AI analysis, landing page audit, marketing automation, form trigger, web scraping, OpenAI, n8n
