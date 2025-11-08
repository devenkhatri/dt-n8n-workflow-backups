# Workflow Analysis for Passport Photo Validator with AI Vision

## Description
This workflow automatically validates passport photos against the UK government's guidelines using an AI vision model. It processes a series of portrait images and determines their suitability, providing reasons for invalidity.

## Input Details
The workflow is manually triggered and processes a predefined list of Google Drive URLs, each pointing to a portrait photo.

## Process Summary
The workflow starts by defining a list of Google Drive URLs for portrait photos. It then iterates through each URL, downloading the corresponding photo from Google Drive. Each downloaded photo is resized to 1024x1024 pixels for optimal AI processing. An AI vision model, specifically Google Gemini, is then used in conjunction with a prompt containing UK government passport photo rules to assess the validity of each photo. Finally, a structured output parser extracts a boolean validity status, a description of the photo, and any reasons for invalidity from the AI's response.

## Output Details
The workflow produces a structured JSON output for each processed photo, detailing whether the photo is valid, a descriptive text of the photo, and an array of reasons if the photo is deemed invalid.
