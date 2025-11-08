# Workflow Analysis for LLM-Powered Article Fact-Checking and Error Summary

## Description
This workflow automates the process of fact-checking an article against provided factual documents. It identifies incorrect statements within the article and generates a structured summary of all detected factual errors, categorizing the article's overall accuracy.

## Input Details
The workflow can be triggered manually for testing or by another workflow, receiving an article's text and a set of reference facts as input.

## Process Summary
1. The workflow begins by receiving an article's content and reference facts, either manually or from another workflow.
2. It then precisely splits the article's text into individual sentences, preserving special formatting like dates or list items.
3. Each sentence is then individually compared against the provided reference facts using a specialized Ollama language model (bespoke-minicheck:latest) to determine its factual accuracy.
4. Only the sentences identified as factually incorrect are filtered and collected.
5. Finally, another Ollama language model (qwen2.5:1.5b) processes the collected incorrect statements to generate a comprehensive summary, including the number of errors, a list of specific incorrect statements, and an overall assessment of the article's factual accuracy.

## Output Details
The workflow produces a detailed, structured summary report outlining the factual inaccuracies found in the input article, along with an overall assessment.
