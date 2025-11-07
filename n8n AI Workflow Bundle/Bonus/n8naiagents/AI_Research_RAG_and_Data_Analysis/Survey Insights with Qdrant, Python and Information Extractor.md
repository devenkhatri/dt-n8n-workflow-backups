# Workflow Analysis for AI-Powered Survey Insight Generator

## Description
This workflow automates the process of extracting detailed insights from survey responses using AI. It imports raw survey data, vectorizes individual responses, identifies clusters of similar answers using K-means clustering, and then leverages a large language model (LLM) to summarize these clusters, extract insights, and determine sentiment for each question. The generated insights are then exported to a new Google Sheet for easy review.

## Input Details
The workflow is manually triggered or initiated by an "Execute Workflow Trigger" node, receiving survey data from a specified Google Sheet.

## Process Summary
First, survey responses are imported from Google Sheets and transformed into question-answer pairs. These pairs are then vectorized using OpenAI embeddings, chunked by a text splitter, and stored in a Qdrant vector database with relevant metadata. A sub-workflow is then triggered to process these stored responses. It dynamically creates a new Google Sheet for insights, fetches all survey questions, and for each question, queries Qdrant to find all corresponding answers. K-means clustering is applied to these answers to identify groups of similar responses, ensuring only clusters with a minimum number of responses are considered. Finally, an OpenAI Chat Model (GPT-4o-mini) analyzes each significant cluster, generating a summary, an insight, and a sentiment score, which are then appended to the newly created Google Sheet.

## Output Details
The workflow produces detailed summaries, insights, and sentiment analyses for clusters of similar survey responses, which are written as new rows to a designated "Insights" sheet within the original Google Spreadsheet.
