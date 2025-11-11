# Workflow Analysis for BannerBear Clone - Social Media Banner Generator

## Description
This workflow allows users to generate custom social media banners for events by filling out a form with event details and an AI image prompt. The system generates an AI image, uploads it to Cloudinary, combines it with event text in a BannerBear template, and posts the final banner to Discord.

## Input Details
The workflow is triggered by a form submission containing event details (title, location, date) and an AI image prompt, along with a template selection.

## Process Summary
1. A user submits a form with event information and an image prompt. 2. The workflow maps the form data to structured parameters, including a template ID. 3. An AI image is generated using OpenAI's DALL-E based on the provided prompt. 4. The generated image is uploaded to Cloudinary for hosting. 5. The image URL and event text are sent to BannerBear to generate a social media banner using a predefined template, and the final image is posted to a Discord channel.

## Output Details
The workflow produces a customized social media banner image and posts it to a specified Discord channel with a message containing event details.

## Tags
banner generation, AI image, social media, Discord, Cloudinary, BannerBear, form automation, event promotion
