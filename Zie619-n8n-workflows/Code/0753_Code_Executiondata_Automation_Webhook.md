# Workflow Analysis for Luma AI Dream Machine - Simple v1 - AK

## Description
This workflow generates AI-powered videos using Luma AI's Dream Machine by combining a user-defined prompt with a randomly selected camera motion, then logs the video generation details in an Airtable database.

## Input Details
The workflow is triggered manually via the 'Test workflow' button and uses predefined settings for video generation.

## Process Summary
The workflow starts with a manual trigger, then defines global settings including the video prompt, aspect ratio, duration, and other parameters. A random camera motion is selected from a predefined list. These settings are combined and sent via an HTTP POST request to the Luma AI API to generate a video. Once the video generation is complete, the response data is captured and used to create a new record in an Airtable table with details like generation ID, prompt, model, resolution, and status.

## Output Details
The workflow creates a new record in an Airtable base containing metadata about the generated video, including its ID, prompt, aspect ratio, duration, resolution, and status.

## Tags
Luma AI, text-to-video, AI video generation, Airtable integration, automation, camera motion, video production, n8n workflow
