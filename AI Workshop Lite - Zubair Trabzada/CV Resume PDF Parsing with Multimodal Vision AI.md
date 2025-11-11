# Workflow Analysis for AI-Powered Resume Screening with Vision Model

## Description
This workflow evaluates candidate resumes for a specific job role by converting the PDF resume into an image and analyzing it with a multimodal AI model (Google Gemini). It's designed to detect and ignore hidden prompts or manipulative content that may be embedded in resumes to bypass traditional text-based screening systems.

## Input Details
The workflow is manually triggered and downloads a candidate's resume PDF from Google Drive.

## Process Summary
First, the workflow downloads a resume PDF from Google Drive. It then converts the PDF into a JPG image using the Stirling PDF API and resizes the image to 75% of its original size for faster processing. The resized image is analyzed by Google's Gemini multimodal LLM, which evaluates the candidate's qualifications for a plumber role. The LLM's response is parsed into a structured format indicating whether the candidate is qualified and why.

## Output Details
The workflow outputs a structured decision (qualified or not) with reasoning, which can be used to determine if the candidate should proceed to the next hiring stage.

## Tags
resume screening, AI hiring, vision model, PDF to image, Google Gemini, Stirling PDF, ATS bypass protection, multimodal AI
