# Workflow Analysis for Tool - Generate Image

## Description
This workflow generates a custom AI image based on a provided context and title, using strict brand guidelines inspired by The Recap AI Newsletter's watercolor aesthetic. The resulting image is converted to PNG format and shared in a designated Slack channel both as a message and an uploaded file.

## Input Details
The workflow is triggered manually or via another workflow with two inputs: 'imageContext' (a description for the image prompt) and 'imageTitle' (the title of the image).

## Process Summary
First, the workflow sets detailed brand guidelines for image generation, emphasizing a watercolor style with specific texture, color, and composition rules. It then sends a request to OpenAI's image generation API using the provided context and the brand guidelines as part of the prompt. The resulting base64-encoded image is converted into a PNG binary file. Finally, the workflow simultaneously posts a message with the image title and uploads the generated PNG file to a predefined Slack channel.

## Output Details
The workflow outputs a PNG image generated from the provided prompt and shares it in a Slack channel with an accompanying message containing the image title.

## Tags
AI image generation, OpenAI, Slack integration, brand guidelines, watercolor style, PNG conversion, workflow automation
