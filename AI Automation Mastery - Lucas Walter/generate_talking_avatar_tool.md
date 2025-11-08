# Workflow Analysis for Generate Talking Avatar Video and Share on Slack

## Description
This workflow automates the creation of a talking avatar video from a script using HeyGen and shares the final video link on a designated Slack channel once it is ready.

## Input Details
This workflow is manually triggered or triggered by another workflow, receiving a text "script" as input.

## Process Summary
First, the workflow receives a text script. It then sends this script to the HeyGen API to initiate the creation of a talking avatar video with a specific avatar, voice, and green background. After initiating the video generation, the workflow enters a loop, periodically checking the video's status with HeyGen until it confirms the video generation is "completed". Once completed, the workflow extracts the video URL.

## Output Details
The workflow sends the URL of the generated talking avatar video to a specified Slack channel.
