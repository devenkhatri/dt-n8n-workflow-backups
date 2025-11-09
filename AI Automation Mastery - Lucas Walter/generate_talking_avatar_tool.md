# Workflow Analysis for Tool - Generate Talking Avatar

## Description
This workflow generates a talking avatar video using HeyGen based on a provided script, waits for the video to be processed, checks its status repeatedly until completion, and then shares the final video URL in a Slack channel.

## Input Details
The workflow is triggered manually or by another workflow and receives a 'script' input containing the text the avatar should speak.

## Process Summary
The workflow starts by accepting a script input, then sends a request to HeyGen's API to generate a talking avatar video with predefined avatar and voice settings. It waits for a period before checking the video generation status via another API call. If the video isn't ready, it loops back to wait and check again. Once the video status is 'completed', it proceeds to share the video URL in a specified Slack channel.

## Output Details
The workflow posts the completed talking avatar video URL to a designated Slack channel for immediate access by users.

## Tags
heygen, avatar, video generation, slack, ai video, talking avatar, content creation
