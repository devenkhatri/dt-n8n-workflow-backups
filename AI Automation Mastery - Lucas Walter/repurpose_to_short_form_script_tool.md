# Workflow Analysis for Repurpose Video to Short-Form Script through AI

## Description
This workflow automates the process of generating short-form video scripts from long-form video content using AI. It takes a video URL as input, extracts its transcript, and then leverages AI models to condense the content into engaging short-form scripts, complete with hooks, calls to action, and relevant hashtags.

## Input Details
The workflow is triggered by an HTTP request, receiving a video URL as input to initiate the script generation process.

## Process Summary
First, the workflow extracts the transcript from the provided video URL using a custom Python script. Next, it sends this transcript to an AI model to generate multiple short-form script ideas, including hooks and calls to action. Subsequently, another AI model refines these ideas into finalized short-form scripts. Finally, a separate AI model generates relevant hashtags for the refined scripts.

## Output Details
The workflow outputs a collection of short-form video scripts, each including a hook, a call to action, and relevant hashtags, directly in the HTTP response.
