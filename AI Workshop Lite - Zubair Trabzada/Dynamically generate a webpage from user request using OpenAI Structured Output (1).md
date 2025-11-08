# Workflow Analysis for Dynamically Generate HTML Page with OpenAI Structured Output

## Description
This workflow demonstrates how to dynamically create an HTML webpage using a user's text query, leveraging OpenAI's structured output capabilities and Tailwind CSS for styling. It showcases the ability to guarantee a specific JSON output format from OpenAI, which is then transformed into a complete HTML page.

## Input Details
The workflow is triggered by an HTTP webhook that receives a user query as a URL parameter.

## Process Summary
First, the user's query is sent to OpenAI with a system prompt to act as a UI designer, requesting a structured JSON output defining HTML components with Tailwind attributes. Next, a second OpenAI call converts this structured JSON into raw HTML content and a page title. This generated HTML and title are then embedded into a complete HTML document that includes the Tailwind CSS framework.

## Output Details
The workflow responds to the initial webhook request by returning the dynamically generated HTML page to the user.
