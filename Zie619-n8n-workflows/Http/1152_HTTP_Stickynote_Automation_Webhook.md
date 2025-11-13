# Workflow Analysis for OpenAI ImageGen1 Template

## Description
This workflow generates AI-edited images using OpenAI's Image Generation API based on a user-provided text prompt and source image. It’s designed to be part of a larger system for selling customized AI-generated images, with built-in support for file handling and integrations with storage, messaging, or payment platforms.

## Input Details
The workflow is triggered manually or via a chat message containing a text prompt and an uploaded source image.

## Process Summary
The workflow starts by receiving a chat message with a text prompt and an image file. It then sets an OpenAI API key, sends a POST request to the OpenAI ImageGen v1 API with the prompt and image, and receives a base64-encoded generated image in response. This response is converted into a binary file for further use. Error handling is applied at multiple steps to ensure robustness.

## Output Details
The workflow outputs a generated image file that can be sent via email, stored in cloud storage, or shared on messaging platforms like Slack or Discord.

## Tags
OpenAI, image generation, AI, n8n, automation, file processing, API integration, production-ready
