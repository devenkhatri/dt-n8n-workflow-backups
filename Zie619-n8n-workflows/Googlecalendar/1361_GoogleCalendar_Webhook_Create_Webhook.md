# Workflow Analysis for Build a Chatbot, Voice Agent and Phone Agent with Voiceflow, Google Calendar and RAG

## Description
This workflow powers a smart assistant that can handle customer inquiries via chat, voice, or phone by integrating Voiceflow with Google Calendar for appointment booking, an external order tracking system, and a Retrieval-Augmented Generation (RAG) system that pulls relevant information from a company knowledge base stored in a Qdrant vector database.

## Input Details
The workflow is triggered by three separate webhooks: one for order status inquiries, one for appointment scheduling, and one for general knowledge questions that require RAG lookup.

## Process Summary
The workflow processes three types of requests: (1) For order inquiries, it calls an external tracking API and returns the order status; (2) For appointment requests, it parses the appointment date, formats it for Google Calendar, and creates a calendar event; (3) For general questions, it uses a RAG system that retrieves relevant documents from a Qdrant vector store (populated from Google Drive files) and generates AI-powered responses using OpenAI's GPT-4o-mini model. Each branch ends with a webhook response to the original requester.

## Output Details
The workflow sends back appropriate responses via webhooks: order status details, appointment confirmation messages, or AI-generated answers to questions based on company knowledge.

## Tags
chatbot, voice agent, phone agent, Voiceflow, Google Calendar, RAG, Qdrant, OpenAI, order tracking, appointment scheduling, n8n, automation
