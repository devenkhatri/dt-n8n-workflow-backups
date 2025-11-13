# Workflow Analysis for 🐋DeepSeek V3 Chat & R1 Reasoning Quick Start

## Description
This workflow is an automated system demonstrating various methods to interact with DeepSeek V3 Chat and R1 Reasoning AI models, along with a local Ollama DeepSeek model, including direct API calls and an AI conversational agent with memory.

## Input Details
The workflow is triggered manually or by receiving chat messages, providing a chatInput for AI processing.

## Process Summary
The workflow starts either manually or upon receiving a chat message. It then branches into several paths: one path uses an AI Agent with window buffer memory for conversational interactions with DeepSeek. Another path directly calls the DeepSeek API via HTTP requests, demonstrating both DeepSeek Chat V3 and DeepSeek Reasoner R1 models. Additionally, it shows integration with a local Ollama DeepSeek-R1 model for AI processing. Informative sticky notes throughout the workflow provide documentation and configuration details for connecting to DeepSeek APIs.

## Output Details
The workflow generates AI-driven responses from DeepSeek V3 Chat, DeepSeek R1 Reasoner, and Ollama DeepSeek models, which are typically returned as API responses or utilized within the ongoing conversational context.

## Tags
automation, n8n, production-ready, excellent, optimized
