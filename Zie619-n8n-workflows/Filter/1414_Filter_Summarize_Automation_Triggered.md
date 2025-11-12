# Workflow Analysis for Store Notion's Pages as Vector Documents into Supabase with OpenAI

## Description
This workflow automatically captures new pages added to a Notion database, extracts their textual content, converts it into vector embeddings using OpenAI, and stores the embeddings along with metadata in a Supabase table that supports vector columns.

## Input Details
The workflow is triggered when a new page is added to a specified Notion database, receiving the page's metadata and URL.

## Process Summary
The workflow starts by detecting a newly added Notion page. It retrieves all blocks from the page, filters out non-text elements like images and videos, and concatenates the remaining text content. This text is then enriched with metadata (like page ID and title) and split into smaller chunks. OpenAI generates embeddings for these chunks, which are then stored in a Supabase table with a vector column.

## Output Details
The processed text chunks and their corresponding OpenAI-generated vector embeddings, along with Notion page metadata, are inserted into a Supabase database table.

## Tags
Notion, Supabase, OpenAI, vector embeddings, automation, document processing, n8n, production-ready
