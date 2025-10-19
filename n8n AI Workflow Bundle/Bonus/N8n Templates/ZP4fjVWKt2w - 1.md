# Workflow Analysis for AI Text Summarizer (5 Bullet Points)

## Description
This workflow demonstrates how to use an Artificial Intelligence model (OpenAI) to take a block of text, summarize it, and restructure the output into a clear, concise list of five bullet points. It is an excellent template for quick content synthesis.

## Input Details
The workflow is triggered manually and uses dummy text data defined in a preceding 'Set' node.

## Process Summary
The workflow starts with a manual execution, followed by a 'Set' node that defines the initial text variable. Next, an OpenAI (Chat) node receives the text and is instructed via a prompt to summarize it into exactly five bullet points. The result from the AI is then captured by another 'Set' node, which stores the summary. Finally, the processed summary is returned as the final output.

## Output Details
The workflow produces a five-point bulleted summary of the input text, which is returned as the final output.
