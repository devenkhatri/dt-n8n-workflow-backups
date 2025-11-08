# Workflow Analysis for Research Agent Demo

## Description
This workflow demonstrates an AI-powered research agent that can answer user queries by leveraging multiple information sources like Wikipedia, Hacker News, and SerpAPI.

## Input Details
The workflow is triggered manually or by an internal system, receiving a research query as input, such as a request for articles on a specific topic.

## Process Summary
The workflow starts by receiving a research query. An AI research agent, powered by an OpenAI chat model, then analyzes the query and decides which tool to use among Wikipedia, Hacker News, or SerpAPI to find the answer. It prioritizes Wikipedia first, then Hacker News, and finally SerpAPI. The Hacker News tool's search parameters (limit and keyword) are dynamically set by the AI. Once the agent finds an answer using one of the tools, the workflow concludes.

## Output Details
The workflow produces a comprehensive answer or relevant information based on the initial research query, which is then made available as a response.
