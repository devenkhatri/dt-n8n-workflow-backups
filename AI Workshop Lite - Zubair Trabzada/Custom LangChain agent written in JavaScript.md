# Workflow Analysis for LangChain - Example - Code Node Example

## Description
This workflow demonstrates how to use custom code nodes in n8n with LangChain to create both a simple LLM chain and an AI agent that can query Wikipedia. It shows two different ways to interact with language models—direct prompting and tool-augmented reasoning.

## Input Details
The workflow is triggered manually by clicking 'Execute Workflow' and does not receive external input data.

## Process Summary
The workflow starts with a manual trigger that splits into two paths. The first path sets a prompt asking for a joke, passes it to a custom LLM chain node that uses an OpenAI model to generate a response. The second path sets a question about Einstein's birth year, which is sent to an AI agent that uses a custom Wikipedia tool (via a code node) and a Chat OpenAI model to look up and return the answer.

## Output Details
The workflow produces two outputs: a generated joke from the LLM chain and a factual answer from the AI agent using Wikipedia, both available in the execution result within n8n.

## Tags
LangChain, OpenAI, AI Agent, LLM Chain, Custom Code Node, Wikipedia Tool, Manual Trigger
