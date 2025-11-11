# Workflow Analysis for Manualtrigger Workflow

## Description
This workflow automatically generates LinkedIn promotional posts for recent blog articles by pulling content from a Ghost blog, cleaning the HTML, and using an AI assistant to create engaging messages tailored for professionals. The results—including original article data and AI-generated LinkedIn posts—are saved to a Google Sheet for review and scheduling.

## Input Details
The workflow is manually triggered and fetches the latest blog posts (up to 3) from a Ghost CMS instance.

## Process Summary
The workflow starts by manually triggering the process, then fetches recent blog posts from Ghost including their HTML content, title, URL, and featured image. It extracts and structures key metadata from each post. A loop processes each article individually, cleaning the HTML content into plain text. This clean content, along with the title and link, is sent to an AI agent (using GPT-4o-mini) with a custom prompt to generate a professional LinkedIn post. The cleaned content and AI-generated message are merged with the original post data and appended to a Google Sheet.

## Output Details
The workflow outputs structured data for each blog post—including the AI-generated LinkedIn message—into a Google Sheet for content planning and publishing.

## Tags
Ghost, LinkedIn, AI, content marketing, Google Sheets, blog automation, OpenAI, n8n, manual trigger, content generation
