# Workflow Analysis for Text Processing and AI Analysis Workflow

## Description
This workflow serves as an ETL pipeline designed to extract text data from a specified directory, process it through an AI model for analysis, and then store the processed information.

## Input Details
This workflow is manually triggered and uses a "Read Files in Directory" and "Split In Batches" nodes as its initial data source.

## Process Summary
The workflow starts by reading text files from a local directory. It then processes these files in batches, sending the content of each file to an AI model for analysis. The AI model determines the sentiment of the text and extracts keywords. Finally, the workflow stores the original text, the sentiment, and the extracted keywords.

## Output Details
The workflow outputs the original text, its sentiment, and extracted keywords, which can then be used for further analysis or storage.
