# Workflow Analysis for AI Tech Newsletter Generator

## Description
This workflow automates the creation and distribution of an AI technology newsletter by gathering articles, generating summaries and social media posts, and then sending it to a mailing list.

## Input Details
The workflow is triggered manually, allowing the user to initiate the newsletter generation process on demand.

## Process Summary
First, the workflow fetches the latest AI tech articles from a Google Sheet. Next, it iterates through each article, using an AI model to generate a concise summary and relevant social media posts. Then, it uses a custom HTML template to format the newsletter content, incorporating the summarized articles and social media posts. Finally, it sends the personalized newsletter to a predefined mailing list.

## Output Details
The workflow sends a personalized AI technology newsletter to a predefined mailing list via an email service.
