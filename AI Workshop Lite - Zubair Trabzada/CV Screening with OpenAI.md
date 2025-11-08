# Workflow Analysis for CV Screening with OpenAI

## Description
This workflow automates the initial screening of CVs by downloading a resume, extracting its content, and sending it to OpenAI for detailed analysis against a given job description. It generates a structured evaluation including a suitability score and detailed reasons for fit or unsuitability.

## Input Details
The workflow is manually triggered and receives a CV file URL and a job description as its primary input.

## Process Summary
1. The workflow is manually triggered and initializes variables including a CV file URL, job description, and parameters for OpenAI analysis. 2. It proceeds to download the CV from the specified URL. 3. The downloaded PDF document's text content is then extracted. 4. This extracted text, combined with the job description and a custom prompt, is sent to OpenAI's chat completion API. 5. OpenAI processes the information and returns a structured JSON response based on a defined schema, evaluating the candidate's suitability. 6. The workflow concludes by parsing this JSON response into a usable data structure.

## Output Details
The workflow produces a parsed JSON object containing a comprehensive candidate evaluation, including a suitability percentage, a summary, and lists of reasons why the candidate is suitable or not suitable for the job.
