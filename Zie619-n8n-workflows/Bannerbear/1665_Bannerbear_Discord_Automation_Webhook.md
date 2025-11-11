# Workflow Analysis for BannerBear Clone - AI-Powered Social Media Banner Generator

## Description
This workflow allows users to generate custom social media banners by filling out a form with event details and an AI image prompt. It uses AI to create an image, uploads it to a cloud service, applies the image and text to a customizable template via BannerBear, and posts the final banner to Discord.

## Input Details
The workflow is triggered by a web form submission that collects event details (title, location, date), a template choice, and an image prompt.

## Process Summary
1. A form is filled out with event details and an image prompt. 2. The form data is processed to map template names to IDs and extract event fields. 3. An AI image is generated using OpenAI DALL·E based on the provided prompt. 4. The generated image is uploaded to Cloudinary for hosting and optimization. 5. The image URL and event text are sent to BannerBear to generate a branded social media banner, which is then posted to a Discord channel.

## Output Details
The final social media banner image is posted to a specified Discord channel with a message containing event details.

## Tags
AI image generation, social media automation, BannerBear, Cloudinary, Discord, n8n forms, OpenAI, event marketing
