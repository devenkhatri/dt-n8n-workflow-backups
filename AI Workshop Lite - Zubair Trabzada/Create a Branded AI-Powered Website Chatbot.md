# Workflow Analysis for Branded AI-Powered Website Chatbot Creation

## Description
This workflow automates the creation of a branded AI-powered website chatbot by leveraging user input for chatbot persona, scraped website content, and OpenAI API.

## Input Details
This workflow is manually triggered and receives inputs for website URL, chatbot name, model temperature, and system message to define the chatbot's persona.

## Process Summary
The workflow starts by scraping content from the provided website URL. This content is then prepared and chunked into smaller pieces. Subsequently, a Pinecone index is upserted with this processed data. Finally, a custom chatbot instruction containing all the information is sent to the AI Model.

## Output Details
The workflow outputs a branded AI-powered website chatbot that is trained on the provided website content and operates according to the defined persona and instructions.
