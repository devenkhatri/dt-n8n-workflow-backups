# Workflow Analysis for AI-Powered Resume Screening with Vision LLM

## Description
This workflow automatically evaluates candidate resumes by converting them from PDF to images and analyzing them with a vision-capable AI model to determine if they qualify for the next hiring stage, while also defending against hidden AI manipulation prompts embedded in resumes.

## Input Details
The workflow is manually triggered and begins by downloading a specific candidate resume PDF from Google Drive.

## Process Summary
The workflow starts by downloading a candidate's resume PDF from Google Drive. It then converts the PDF into a JPEG image using the Stirling PDF API and resizes the image to 75% of its original dimensions for efficient processing. The resized image is passed to Google's Gemini multimodal LLM along with a prompt asking it to evaluate the candidate's suitability for a Plumber role. The LLM returns a structured response indicating whether the candidate is qualified and the reasoning behind the decision. Finally, the workflow checks the 'is_qualified' boolean to determine if the candidate should proceed to the next hiring stage.

## Output Details
The workflow outputs a structured decision (qualified or not) with reasoning, which can be used to automatically filter candidates for further interview stages.

## Tags
resume screening, AI hiring, vision LLM, PDF to image, Google Gemini, ATS bypass prevention, multimodal AI, candidate evaluation, n8n workflow, Google Drive
