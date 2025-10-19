# Workflow Analysis for RAG Workflow Comparison: Direct RAG vs. RAG Agent

## Description
This workflow demonstrates and compares two distinct methods for implementing Retrieval-Augmented Generation (RAG): a traditional, explicit RAG workflow and a more dynamic, tool-using RAG Agent. It shows how to retrieve context from a knowledge base and use it to generate a grounded, factual answer using a Large Language Model (LLM).

## Input Details
The workflow is likely initiated by a Manual Trigger and requires a user's question or query as input data.

## Process Summary
The workflow starts with an input query and then proceeds through two parallel paths: a RAG Workflow and a RAG Agent. The RAG Workflow path first uses a Vector Store node to retrieve relevant documents, combines the context with the query, and sends it to a Chat Model to generate the answer. The RAG Agent path initializes an LLM Agent, which dynamically decides to use a Vector Store tool to retrieve context before generating a response. Finally, both results are outputted for review.

## Output Details
The workflow produces two generated responses—one from the direct RAG workflow and one from the RAG Agent—which are returned as the final output for comparison.
