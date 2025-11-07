# Workflow Analysis for Make OpenAI Citation for File Retrieval RAG

## Description
This workflow leverages an OpenAI assistant with file retrieval capabilities to generate responses with accurate citations from vector store files. It addresses issues where the assistant might produce unformatted citations or strange characters, allowing for dynamic referencing (e.g., citation 1, 2, 3) and formatting the output using Markdown or HTML.

## Input Details
The workflow is triggered by a chat interface within n8n, receiving user queries as input.

## Process Summary
1. A user's chat message triggers the workflow, which is then sent to a pre-configured OpenAI assistant with an attached vector store for file retrieval.
2. The workflow then makes an HTTP request to OpenAI to retrieve all messages from the conversation thread, as the initial assistant response may not include all citation details.
3. The retrieved thread content is split to extract individual messages, their content, and specifically, the file citations embedded within the text.
4. For each citation, another HTTP request fetches the corresponding filename from OpenAI using the file ID.
5. Finally, a code node replaces the original citation placeholders in the assistant's output with a formatted reference including the retrieved filename.

## Output Details
The workflow produces a human-readable response from the OpenAI assistant, with citations formatted to include the relevant filenames, which is then returned to the chat interface.
