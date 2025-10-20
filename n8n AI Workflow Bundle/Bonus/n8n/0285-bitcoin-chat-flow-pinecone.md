# Workflow Analysis for Bitcoin Chat Flow with Pinecone

## Description
This workflow enables a chatbot to answer questions about Bitcoin by leveraging Pinecone for vectorized search and OpenAI for generating conversational responses.

## Input Details
The workflow is triggered by an HTTP request, expecting a "message" in the request body.

## Process Summary
The workflow receives a user message via HTTP. It then converts the message into an embedding using OpenAI. This embedding is used to query Pinecone, retrieving the top 5 most similar Bitcoin-related documents. The retrieved documents are summarized and combined with the original user message to formulate a detailed prompt for OpenAI. Finally, OpenAI generates a conversational response based on this prompt.

## Output Details
The workflow returns a conversational response from OpenAI as an HTTP response.
