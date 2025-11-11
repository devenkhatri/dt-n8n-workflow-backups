# Workflow Analysis for Passport Photo Validator

## Description
This workflow validates whether uploaded portrait photos meet the UK government's passport photo requirements using an AI vision model. It checks aspects like background, facial visibility, image quality, and other official criteria, then returns a structured response indicating validity along with reasons and photo descriptions.

## Input Details
The workflow is manually triggered and uses a predefined list of Google Drive photo URLs as input for validation.

## Process Summary
The workflow begins by defining a list of photo URLs from Google Drive. Each photo is downloaded, resized to a maximum of 1024x1024 pixels if larger, and then passed to an AI vision model (Google Gemini) for analysis. The AI evaluates the image against UK passport photo rules and returns a structured output indicating whether the photo is valid, a description of the image, and the reasons for the decision.

## Output Details
The workflow produces a structured JSON response for each photo indicating its validity, a description of its contents, and a list of reasons based on UK passport guidelines, which can be used to update a database or application backend.

## Tags
AI Vision, Passport Photo Validation, Google Drive, Image Processing, Structured Output, Google Gemini, Workflow Automation
