# Workflow Analysis for HackerNews Learning Resource Workflow

## Description
This workflow collects user input on a topic they want to learn, searches for relevant discussions on HackerNews, analyzes the comments to identify top resources, and emails the user with the findings.

## Input Details
The workflow is triggered by a form submission where users input their email and the topic they want to learn.

## Process Summary
The workflow searches HackerNews for discussions related to the user's topic, extracts comments from these discussions, analyzes them using a language model to identify top resources, categorizes these resources, and performs sentiment analysis. It then formats the results in Markdown and converts it to HTML. Finally, it emails the user with the top resources.

## Output Details
The workflow sends an email to the user with the top resources to learn their desired topic, categorized and formatted in HTML.
