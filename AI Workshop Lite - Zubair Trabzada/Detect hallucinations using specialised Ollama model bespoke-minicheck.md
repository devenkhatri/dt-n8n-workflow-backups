# Workflow Analysis for Hallucination Detection with Ollama

## Description
This workflow analyzes text input using a specialized Ollama model to detect and flag potential hallucinations, providing a confidence level for the detection.

## Input Details
The workflow is triggered manually and takes text as input from a "Hallucination Input" node.

## Process Summary
The workflow starts by receiving text input. It then prepares a prompt for the Ollama model, instructing it to detect hallucinations and provide a confidence level between 0 and 1. This prompt, along with the received text, is sent to the Ollama model. Finally, the model's response, which includes the hallucination detection and confidence, is processed to extract and display the key information.

## Output Details
The workflow outputs the Ollama model's response, specifically highlighting whether hallucinations were detected and the confidence level, in a human-readable format.
