# Workflow Analysis for Tool - Generate Talking Avatar

## Description
This workflow creates a talking avatar video using a provided script, waits for the video to be processed, checks its status repeatedly until completion, and then shares the final video link in a specified Slack channel.

## Input Details
The workflow is triggered manually or via another workflow with a 'script' input containing the text the avatar should speak.

## Process Summary
The workflow starts by receiving a script input. It sends a request to the HeyGen API to generate a talking avatar video with a predefined avatar, voice, and green background. After initiating the video generation, it waits for a period before checking the video's processing status. If the video is not yet completed, it loops back to wait and check again. Once the video status shows as 'completed', it posts the video URL to a designated Slack channel.

## Output Details
The workflow outputs a message with the completed talking avatar video URL posted to a specific Slack channel.

## Tags
avatar, video generation, HeyGen, Slack, AI video, automation
