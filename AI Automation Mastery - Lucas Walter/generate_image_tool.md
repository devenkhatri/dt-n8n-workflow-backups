# Workflow Analysis for Tool - Generate Image

## Description
This workflow generates a branded, AI-created image based on a provided context and title, following specific visual guidelines for The Recap AI Newsletter. It uses OpenAI's image generation API to create a customized watercolor-style image and shares it in a designated Slack channel.

## Input Details
The workflow is triggered manually or via another workflow with two inputs: 'imageContext' (a description guiding the image content) and 'imageTitle' (a title for the generated image).

## Process Summary
The workflow starts by receiving image context and title inputs. It then sets detailed brand guidelines for a watercolor-style image suitable for The Recap AI Newsletter. These guidelines and the image context are sent to OpenAI's image generation API to create the image. The resulting base64-encoded image is converted into a binary PNG file. Finally, the workflow posts a message with the image title and uploads the generated image to a specific Slack channel.

## Output Details
The workflow outputs a generated PNG image and posts both a descriptive message and the image file to a predefined Slack channel (C08KC39K8DR).

## Tags
image generation, OpenAI, Slack integration, branding, automation, marketing, AI art, watercolor style
