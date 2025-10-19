# Workflow Analysis for OpenAI Chaining - Summarize Generated Text

## Description
This workflow demonstrates chaining two OpenAI operations: first, it generates content based on a prompt, and second, it uses the generated content as input for a subsequent prompt, such as summarization. This is useful for complex AI tasks where multiple steps of processing are required.

## Input Details
The workflow is triggered manually and uses hardcoded variables (`prompt` and `model`) defined within a Code node for initial testing input.

## Process Summary
The workflow starts manually and initializes testing variables (`prompt` and `model`) in a Code node. The first OpenAI node generates a response using the initial prompt via the Chat Completion model. The second OpenAI node takes the output from the previous step and prompts the model to summarize that text in a single sentence. Finally, a Set node extracts the resulting summarized text content from the second API response and assigns it to a variable named 'summary'.

## Output Details
The workflow produces a variable named `summary` containing the one-sentence summary of the text generated in the first OpenAI step.
