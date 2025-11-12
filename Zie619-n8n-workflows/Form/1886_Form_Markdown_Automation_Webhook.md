# Workflow Analysis for 🤖 On-Page SEO Audit

## Description
This workflow automatically performs a comprehensive on-page SEO audit of a website URL provided by the user. It analyzes both technical SEO elements (like HTML structure) and content quality (like keyword usage and readability), then compiles the findings into a detailed report sent via email.

## Input Details
The workflow is triggered by a web form where the user submits a landing page URL to audit.

## Process Summary
The workflow starts by accepting a landing page URL via a form. It then fetches the page's HTML content using an HTTP request. The raw HTML is sent to two separate AI-powered analysis branches: one performs a technical SEO audit of the page's code, and the other evaluates the content for SEO quality and readability. The results from both audits are merged, formatted into a structured Markdown report, converted to HTML, and finally emailed to a predefined address with the original URL in the subject line.

## Output Details
The workflow generates a combined technical and content SEO audit report in HTML format and sends it as the body of an email via Gmail.

## Tags
SEO, on-page audit, AI analysis, content optimization, technical SEO, website audit, n8n, automation, email report, OpenAI
