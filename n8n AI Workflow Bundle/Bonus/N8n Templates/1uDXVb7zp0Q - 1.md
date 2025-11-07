# Workflow Analysis for Prompting Cheat Sheet

## Description
This workflow serves as a comprehensive guide and demonstration for various advanced prompting techniques and AI agent configurations using large language models within n8n. It showcases methods to improve AI consistency, accuracy (through techniques like Chain-of-Thought, Self-consistency, Step-Back, and ReAct), and output reliability.

## Input Details
The workflow is triggered manually for demonstration purposes with predefined input data, such as example emails and support requests, or by a chat message for the "ReAct" agent section.

## Process Summary
The workflow demonstrates various AI prompting techniques, beginning with consistent email routing using an AI agent and structured output. It then showcases Chain-of-Thought for problem-solving and Self-consistency by voting on multiple LLM classifications of a single input for increased accuracy. Further, it applies a Step-Back method where an LLM first deconstructs a complex request before providing a detailed answer and routing decision. Finally, it illustrates a ReAct agent using external tools (calculator, weather, search) for dynamic task execution and incorporates an auto-fixing parser for reliable output.

## Output Details
The workflow produces classified email queues (with confidence scores), structured answers to complex queries, and detailed responses from AI agents that may include calculations, weather data, or search results, all aimed at illustrating different prompting methodologies.
