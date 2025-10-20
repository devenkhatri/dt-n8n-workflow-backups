# Workflow Analysis for Chat Voice Agent with RAG

## Description
This workflow serves as a chat voice agent utilizing Retrieval-Augmented Generation (RAG) to provide informative responses. It integrates speech-to-text for input, a knowledge base for context, and text-to-speech for audible replies, enabling interactive voice conversations.

## Input Details
The workflow is triggered by an HTTP request containing audio data and a chat ID.

## Process Summary
The workflow transcribes spoken input to text, retrieves relevant context from a Pinecone vector database based on the transcribed text, and constructs a detailed prompt for a Large Language Model (LLM). The LLM then generates a comprehensive response using the provided information, and this text response is converted back into speech. Finally, the generated audio is played back to the user.

## Output Details
The workflow responds with synthesized speech (audio data) generated from the LLM's answer.
