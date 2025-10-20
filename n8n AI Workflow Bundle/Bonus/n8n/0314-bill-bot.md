# Workflow Analysis for Bill Bot Workflow

## Description
This workflow automates the process of extracting bill details from an uploaded PDF, sending these details to a large language model for summarization, and then notifying a Telegram chat with the summarized bill information. It is designed to streamline expense management and provide quick insights into incoming bills.

## Input Details
The workflow is triggered by an HTTP request that receives a PDF file via a webhook.

## Process Summary
The workflow starts by receiving a PDF file. It then uses the PDF Extract Text node to extract all text content from the received PDF. This extracted text is then sent to a large language model (LLM) through the HuggingFace Inference API to summarize the bill. Finally, the summarized bill details are formatted into a message and sent to a specified Telegram chat.

## Output Details
The workflow sends a summarized bill message to a Telegram chat.
