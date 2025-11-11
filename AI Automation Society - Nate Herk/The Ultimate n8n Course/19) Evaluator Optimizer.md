# Workflow Analysis for Evaluator-Optimizer

## Description
This workflow generates a personalized biography based on user input, then automatically evaluates and refines it until it meets specific quality criteria—such as including a quote, being light and humorous, and containing no emojis—before saving the final version to Google Docs.

## Input Details
The workflow is triggered when a chat message is received containing information about a person for whom a biography should be created.

## Process Summary
First, the Biography Agent creates an initial draft using the user-provided details. The Evaluator Agent then checks if the draft meets predefined criteria and outputs either 'Finished' or specific feedback. If the biography isn't finished, the Optimizer Agent revises it based on the feedback, and the loop repeats. Once the Evaluator Agent confirms the biography is complete, it is pushed to a Google Doc.

## Output Details
The final, verified biography is saved to a Google Doc.

## Tags
biography, AI agent, content generation, content evaluation, iterative refinement, Google Docs, LLM workflow
