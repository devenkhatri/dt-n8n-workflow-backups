# Workflow Analysis for Tool - Generate Talking Avatar

## Description
This workflow automates the creation of a talking avatar video using the HeyGen API. It takes text, a desired voice, and an avatar as input to produce a video.

## Input Details
The workflow is triggered by an HTTP POST request to the webhook path `/generate-talking-avatar`, expecting `text`, `voiceId`, and `avatarId` in the request body.

## Process Summary
The workflow starts by receiving a POST request to its webhook. It then calls the HeyGen API to create a video source using the provided text and voice ID. Subsequently, it uses the video ID from the source creation and the input avatar ID to generate the talking avatar via another HeyGen API call. Finally, the workflow sends the result of the avatar generation back to the original webhook caller.

## Output Details
The workflow returns the response from the HeyGen API, containing details about the generated talking avatar video, back to the caller of the initial webhook.
