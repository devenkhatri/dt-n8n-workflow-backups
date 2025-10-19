# Workflow Analysis for YouTube Content Strategist with AI

## Description
This workflow acts as an AI-powered YouTube content strategist, generating video ideas, titles, descriptions, and keywords based on a provided topic or existing YouTube video URL.

## Input Details
The workflow is manually triggered and receives a YouTube video URL or a topic as input.

## Process Summary
The workflow starts by determining if a YouTube video URL or a topic was provided. If an existing YouTube video URL is given, it extracts the transcript and generates three new video ideas from it. If a topic is provided, it generates three video ideas directly from the topic. For each video idea, it refines the YouTube video idea, generates three compelling YouTube titles, creates a detailed YouTube video description, and generates 50 YouTube keywords. Finally, it formats all the generated content into a structured JSON output.

## Output Details
The workflow outputs a structured JSON object containing three YouTube video ideas, each with refined ideas, titles, descriptions, and keywords.
