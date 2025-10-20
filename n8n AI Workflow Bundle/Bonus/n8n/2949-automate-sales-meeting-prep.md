# Workflow Analysis for Automated Sales Meeting Preparation with AI

## Description
This workflow automates the preparation for sales meetings by gathering company information and key details, then generating a summarized brief and personalized talking points to help sales representatives prepare efficiently.

## Input Details
The workflow is manually triggered by a user with company and contact information structured as JSON.

## Process Summary
The workflow starts by extracting company and contact information from the input. It then uses Hunter.io to find the company's website and Clearbit to retrieve detailed company data. After that, it searches for recent news articles related to the company using a custom API and summarizes them with an OpenAI model. Finally, it uses another OpenAI model to generate personalized talking points for the sales meeting based on all the gathered information.

## Output Details
The workflow returns a summarized company brief and personalized talking points as a JSON response.
