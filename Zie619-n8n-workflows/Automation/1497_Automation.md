# Workflow Analysis for DeepResearcher Workflow

## Description
This workflow automates in-depth online research by generating search queries, extracting and analyzing content from search results, and producing structured, information-dense learnings using AI. It integrates with Notion to log findings and sources, and supports user-defined research breadth and depth.

## Input Details
The workflow is triggered manually and receives a research query along with optional parameters such as research breadth (number of sources) via a custom web form.

## Process Summary
The workflow begins by accepting a research query through a form, then generates SERP (search engine results page) queries based on the input. It fetches and processes the top organic search results, converts them to markdown, and uses an AI language model to extract up to three unique, detailed learnings. These learnings, along with source URLs, are formatted into structured Notion blocks and appended to a Notion page linked to the original request. The workflow also handles errors, tracks execution status, and supports multi-level research via subworkflows if needed.

## Output Details
The workflow outputs structured research learnings and source links to a Notion page, updates the request status to 'Done', and displays a completion message to the user.

## Tags
research automation, AI-powered analysis, Notion integration, deep research, web scraping, SERP processing, structured output, n8n workflow
