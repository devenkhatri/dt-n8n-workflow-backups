# Workflow Analysis for Professional Content Rewriter via Webhook (GPT-4)

## Description
This workflow accepts text content via a webhook, uses GPT-4 via the OpenAI API to professionally rewrite the content to be 100% unique and engaging, and then returns the newly generated content as an immediate API response.

## Input Details
The workflow is triggered by an incoming HTTP POST request to a webhook endpoint, expecting a JSON body containing the original text in a field named `content`.

## Process Summary
The workflow starts with a Webhook trigger that passes the input content to a Code node, which validates and prepares the data. Next, the OpenAI node utilizes the GPT-4 model with a specific system prompt to rewrite the provided content for uniqueness and professionalism. A subsequent Code node extracts only the generated text from the AI's response. Finally, a Set node cleans up the data structure, keeping only the new content field before responding.

## Output Details
The workflow immediately responds to the initiating webhook request with a 200 status code, returning a JSON body containing the professionally rewritten content.
