# Workflow Analysis for AI Resume Screening with Multimodal LLM

## Description
This workflow converts a candidate's resume from PDF to an image format. It then uses a Vision Language Model (VLM) to analyze the resume image, assess the candidate's suitability for a specific role, and identify any attempts to bypass automated screening systems.

## Input Details
The workflow is initiated manually and downloads a candidate's resume in PDF format from Google Drive.

## Process Summary
First, the workflow downloads a candidate's resume PDF from Google Drive. Next, it converts the PDF into an image using the Stirling PDF API and then resizes the image. Subsequently, a Google Gemini multimodal LLM analyzes the converted resume image based on a defined job role (e.g., Plumber) and assesses the candidate's qualifications. Finally, a structured output parser extracts a boolean "is_qualified" status and a reason from the LLM's response, which is then used by an If node to determine if the candidate should proceed to the next stage.

## Output Details
The workflow determines if a candidate is qualified for an in-person interview, providing a boolean `is_qualified` and a `reason` based on the VLM's assessment.
