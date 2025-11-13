# Workflow Analysis for Production Workflow

## Description
This workflow automatically publishes blog posts to both Medium and Dev.to whenever a new article is submitted via a webhook, such as from a CMS like Strapi.

## Input Details
The workflow is triggered by a POST webhook that receives article data including title, content, and tag from an external system like Strapi.

## Process Summary
The workflow starts when a POST request is received via a secured webhook. It then simultaneously sends the article data to Medium using the Medium API and to Dev.to using an authenticated HTTP POST request. Both posts include the title, markdown-formatted content, and associated tag from the incoming data. If any step fails, the workflow routes to an error handler that stops execution and logs an error message.

## Output Details
The workflow publishes the article to Medium and Dev.to and halts with an error message if any step fails.

## Tags
blog automation, content syndication, Medium API, Dev.to API, webhook trigger, production workflow, n8n
