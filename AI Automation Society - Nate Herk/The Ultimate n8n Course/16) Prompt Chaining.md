# Workflow Analysis for Prompt Chaining

## Description
This workflow uses a sequence of specialized AI agents to generate a high-quality blog post based on a given topic. It first creates an outline, refines it for structure and flow, writes the full blog post, and then saves the result to a Google Doc.

## Input Details
The workflow is triggered when a chat message containing a blog topic is received via a webhook.

## Process Summary
The workflow starts by receiving a blog topic from a chat message. An AI agent generates an initial outline based on the topic. A second AI agent evaluates and refines the outline to ensure it meets key structural criteria. A third AI agent then writes a full blog post using the revised outline. Finally, the completed blog post is saved to a Google Doc.

## Output Details
The final output is a complete blog post saved to a Google Doc using the authenticated Google Docs account.

## Tags
AI, blog writing, prompt chaining, content creation, Google Docs, LLM, outline generation
