# Workflow Analysis for AI Review and Sentiment Analysis to Google Sheets

## Description
This workflow is designed to automate the process of analyzing textual data, such as customer feedback or reviews, utilizing an AI model to extract key information like summaries and sentiment scores, which are then saved to a Google Sheet.

## Input Details
The workflow is initiated by a manual trigger, allowing for on-demand execution.

## Process Summary
The workflow begins with a manual trigger and is designed to process input data that contains customer reviews or text. It utilizes an OpenAI node to analyze the text, extracting a concise summary and determining a sentiment score based on a defined prompt. Following the AI processing, a Set node is used to consolidate and structure the generated output data. Finally, the structured analysis is recorded by appending the data as new rows into a designated Google Sheet.

## Output Details
The final output is a structured set of analyzed data (summaries and sentiment scores) that is appended as new rows into a specified Google Sheet.
