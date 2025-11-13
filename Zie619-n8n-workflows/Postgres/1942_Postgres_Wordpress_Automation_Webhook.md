# Workflow Analysis for RAG & GenAI App With WordPress Content

## Description
This workflow integrates 24 different services to automate tasks for a RAG & GenAI application with WordPress content

## Input Details
The workflow is triggered by a manual trigger and receives data from WordPress posts and pages

## Process Summary
The workflow retrieves WordPress posts and pages, filters out unpublished and protected content, and then stores the documents on Supabase. It also retrieves documents from Supabase based on chat input and uses the AI agent to provide a helpful answer. The workflow then stores the workflow execution id and timestamp on Supabase

## Output Details
The workflow produces a helpful answer to the user's chat input and stores the workflow execution history on Supabase

## Tags
RAG, GenAI, WordPress, automation, Supabase, AI, chatbot
