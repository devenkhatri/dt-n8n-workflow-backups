# Workflow Analysis for Dynamic LLM Selector and Response Generator

## Description
The workflow receives a chat message, dynamically selects an LLM based on a configurable index, generates a polite response, validates the response against quality criteria, and returns the final text while handling errors and updating the index for the next run.

## Input Details
Triggered manually (or via webhook) and receives a chat message payload containing the customer complaint.

## Process Summary
1) The LLM index is set from the incoming data (default 0). 2) A code node retrieves the list of connected LLM resources, reverses it, and selects the model at the given index. 3) The selected LLM generates a response using a predefined prompt based on the chat input. 4) The generated text is validated with a system‑prompt sentiment/quality check. 5) The workflow returns the validated response or an error message and increments the index for the next execution.

## Output Details
Outputs the final response text (or error message) as the workflow result.

## Tags
LLM,dynamic selection,chat response,validation,error handling,automation
