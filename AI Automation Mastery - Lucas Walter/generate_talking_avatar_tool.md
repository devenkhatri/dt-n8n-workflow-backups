# Workflow Analysis for Tool - Generate Talking Avatar

## Description
This workflow generates a talking avatar video using a provided script via the HeyGen API, waits for the video to be processed, checks its status periodically, and shares the final video link in a Slack channel once ready.

## Input Details
The workflow is triggered manually or via another workflow with a 'script' input containing the text the avatar should speak.

## Process Summary
The workflow starts by receiving a script input, then sends a request to HeyGen's video generation API to create a talking avatar video with a predefined avatar, voice, and green background. It then waits for a set time before checking the video processing status. If the video isn't ready, it loops back to wait and check again. Once the video status is 'completed', the workflow posts the video URL to a specified Slack channel.

## Output Details
The workflow outputs a Slack message containing the URL to the completed talking avatar video in a designated channel.

## Tags
heygen, avatar, video generation, slack, ai video, text-to-video
