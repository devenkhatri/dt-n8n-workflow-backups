# Workflow Analysis for Fact-Checking Workflow for Article Sentences

## Description
This workflow checks the factual accuracy of individual sentences in an article by comparing them against a provided set of factual reference data, using specialized AI models to identify incorrect statements and generate a summary report.

## Input Details
The workflow is triggered either manually for testing (with hardcoded facts and text) or by another workflow that provides two inputs: 'facts' (verified reference information) and 'text' (the article content to be fact-checked).

## Process Summary
First, the input text is split into individual sentences while preserving dates and list formats. Each sentence is then evaluated against the reference facts using a specialized fact-checking AI model (bespoke-minicheck) to determine if it is factually correct ('Yes') or incorrect ('No'). The results are filtered to keep only the incorrect statements, which are then aggregated into a single dataset. Finally, a summary report is generated using a general-purpose AI model (qwen2.5) that counts the errors, lists the incorrect statements, and provides an overall assessment of the article's factual accuracy.

## Output Details
The workflow produces a structured summary report detailing the number of factual errors, listing the incorrect statements, and providing an overall accuracy assessment, which can be used by content teams for revision.

## Tags
fact-checking, AI validation, content verification, sentence analysis, LLM, Ollama, article review, data accuracy
