# Workflow Analysis for Planet Slice ASMR Video Generator

## Description
This workflow allows users to select a planet from a form, generates a unique cinematic ASMR video prompt for it, and then creates an ASMR video of the planet being sliced open using an AI video generation service.

## Input Details
The workflow is triggered by a form submission where a user selects a planet from a dropdown.

## Process Summary
Upon form submission, an AI model (GPT-4.1) generates a detailed cinematic ASMR video prompt based on the selected planet, describing its outer surface and internal layers when sliced. This prompt is then sent to Fal.ai's Veo3 service to initiate video creation. The workflow waits for a short period before querying Fal.ai again to retrieve the generated video.

## Output Details
The workflow outputs an API response containing the generated ASMR video (or a link to it) from the Fal.ai service.
