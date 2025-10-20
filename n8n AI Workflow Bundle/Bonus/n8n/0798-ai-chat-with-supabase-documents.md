# Workflow Analysis for AI Chat with Supabase Documents

## Description
This workflow enables an AI to answer questions based on documents stored in a Supabase database. Upload your documents, ask questions, and the AI will provide answers using the relevant document content.

## Input Details
The workflow is triggered manually and receives questions as input.

## Process Summary
The workflow starts by retrieving document embeddings from Supabase that are related to the user's question. It then combines these relevant document chunks with the user's question to create a context. This context is then sent to a large language model (LLM) to generate an answer. Finally, the generated answer is formatted into a conversational response.

## Output Details
The workflow outputs an AI-generated answer to the user's question, based on the Supabase documents.
