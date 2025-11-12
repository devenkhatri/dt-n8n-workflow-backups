# Workflow Analysis for AI-Powered Resume Screening with Vision Model

## Description
This workflow evaluates job candidate resumes by converting PDFs into images and analyzing them with a multimodal AI model to determine if the applicant is qualified for a specific role—helping to prevent manipulation by hidden AI prompts embedded in resumes.

## Input Details
The workflow is triggered manually and begins by downloading a candidate's resume PDF from Google Drive.

## Process Summary
The workflow first downloads a candidate's resume PDF from Google Drive. It then converts the PDF into a JPG image using the Stirling PDF API. The resulting image is resized to 75% of its original dimensions to optimize processing. Next, the image is passed to Google's Gemini 1.5 Pro vision-capable language model, which evaluates the resume against the requirements of a Plumber role. The model returns a structured response indicating whether the candidate qualifies and why.

## Output Details
The workflow outputs a structured decision indicating whether the candidate qualifies for the next stage, which can be used to trigger downstream actions such as sending an email or updating an ATS.

## Tags
resume screening, AI vision model, PDF to image, Google Gemini, ATS bypass prevention, multimodal AI, candidate evaluation, image processing, manual trigger, n8n workflow
