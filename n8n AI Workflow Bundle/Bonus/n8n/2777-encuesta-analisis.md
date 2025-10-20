# Workflow Analysis for Survey Analysis with AI

## Description
This workflow analyzes survey responses using AI to extract key insights and classifications, then stores the processed data in a Google Sheet.

## Input Details
The workflow is triggered by an HTTP POST request containing survey data.

## Process Summary
The workflow starts by extracting and transforming survey responses, focusing on specific questions. It then uses an AI model to classify the sentiment, emotion, and topics of the main survey response. After AI processing, the workflow translates the AI outputs and combines them with the original survey data. Finally, all the processed information is appended as a new row in a Google Sheet.

## Output Details
The workflow appends the original survey data, along with AI-generated sentiment, emotion, and topic classifications, to a specified Google Sheet.
