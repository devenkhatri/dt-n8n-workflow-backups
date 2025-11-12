# Workflow Analysis for Generate AI-Ready llms.txt Files from Screaming Frog Website Crawls

## Description
This workflow automates the creation of an llms.txt file—a structured list of high-quality, indexable web pages—from a Screaming Frog website crawl export. The resulting file helps AI systems discover and prioritize valuable content from a website.

## Input Details
The workflow is triggered by a form submission that includes the website name, a short description, and a Screaming Frog CSV export file (typically internal_html.csv).

## Process Summary
First, the workflow extracts data from the uploaded Screaming Frog CSV file. It then maps key fields like URL, title, meta description, status code, indexability, content type, and word count, supporting multiple languages. Next, it filters URLs to keep only those that are indexable, return a 200 status, and have HTML content. Optionally, an AI-powered classifier (disabled by default) can further refine content quality. Finally, it formats each valid page as a Markdown-style link with an optional description, concatenates all rows, and prepends the site name and description to create the llms.txt content.

## Output Details
The workflow generates a downloadable llms.txt file containing a formatted list of relevant URLs, ready for use by AI systems or LLMs.

## Tags
automation, SEO, AI, Screaming Frog, llms.txt, content indexing, n8n, text processing, file generation, web crawling
