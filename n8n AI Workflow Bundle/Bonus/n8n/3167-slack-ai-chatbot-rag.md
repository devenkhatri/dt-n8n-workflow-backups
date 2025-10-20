# Workflow Analysis for Slack AI Chatbot with RAG

## Description
This workflow creates a Slack AI chatbot that answers user questions using Retrieval Augmented Generation (RAG) by searching a knowledge base and summarizing the results.

## Input Details
The workflow is triggered by Slack messages containing specific keywords (questions for the AI).

## Process Summary
The workflow extracts the message text and searches a knowledge base (Pinecone) for relevant information. It then uses a language model (Cohere) to generate a summary of the retrieved information. Finally, it formats the response and sends it back to the user in Slack.

## Output Details
The workflow posts the AI-generated answer as a reply in the Slack channel where the question was asked.
