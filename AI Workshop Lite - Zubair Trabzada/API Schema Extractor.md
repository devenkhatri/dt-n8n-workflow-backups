# Workflow Analysis for API Schema Extractor and Documentation Generator

## Description
This workflow extracts API schemas from an OpenAPI specification, generates documentation for each endpoint using AI, and saves the schema and documentation into separate files for each endpoint.

## Input Details
The workflow is manually triggered and receives an OpenAPI JSON schema as input.

## Process Summary
The workflow first extracts a list of endpoints from the provided OpenAPI JSON. For each endpoint, it generates a schema and descriptive documentation using an AI model. Finally, it cleans up unnecessary data and saves the extracted schema and generated documentation into separate JSON and Markdown files, respectively, for each endpoint.

## Output Details
The workflow outputs a collection of JSON files containing API schemas and Markdown files with generated documentation, organized by endpoint.
