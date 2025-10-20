# Workflow Analysis for Web Query Semantic Re-ranking

## Description
This workflow takes a user query and a list of URLs, then uses AI to semantically re-rank the URLs based on their relevance to the query.

## Input Details
The workflow is triggered manually and receives a user query as text and a list of URLs as input.

## Process Summary
First, the workflow takes the user query and URLs. Then, for each URL, it scrapes the content of the webpage. After scraping, it uses an AI model to embed the user query and the content of each webpage into a vector space. Finally, it calculates the cosine similarity between the query embedding and each webpage embedding to determine relevance and re-ranks the URLs based on these scores.

## Output Details
The workflow outputs a re-ranked list of URLs based on their semantic relevance to the input query.
