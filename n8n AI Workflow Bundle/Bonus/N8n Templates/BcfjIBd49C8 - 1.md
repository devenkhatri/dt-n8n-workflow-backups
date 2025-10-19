# Workflow Analysis for Google Sheets Similarity Search & AI Answer Generator

## Description
This workflow creates an AI-powered Question-Answering system by using a Google Sheet as a knowledge base. It triggers on a webhook query, searches the spreadsheet for the most similar entries using a custom similarity function, feeds the top results as context to an OpenAI model, and returns the AI-generated answer.

## Input Details
The workflow is triggered by an incoming HTTP POST request to a webhook, expecting a JSON body containing the user's search query.

## Process Summary
The workflow starts upon receiving a query via a webhook, which is then stored for processing. It retrieves all data from a specified Google Sheet and calculates a string similarity score between the incoming query and each row of the sheet using a custom function. The results are sorted by similarity score, and the top 5 most relevant items are selected and aggregated. Finally, a detailed prompt is built using the original query and the aggregated context before being sent to the OpenAI model for a response.

## Output Details
The workflow returns the AI-generated response, based on the Google Sheet context, directly to the calling webhook endpoint.
