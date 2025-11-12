# Workflow Analysis for Calculate the Centroid of a Set of Vectors

## Description
This workflow calculates the centroid (average point) of a set of numerical vectors provided via a web request. It validates that all vectors have consistent dimensions before computing the average across each dimension.

## Input Details
The workflow is triggered by a GET request to a webhook URL with a query parameter 'vectors' containing a JSON-formatted array of numerical vectors.

## Process Summary
The workflow begins by receiving a GET request with a 'vectors' query parameter. It parses and extracts this parameter into a usable array format. Then, it validates that the input is a non-empty array and that all vectors have the same number of dimensions. If validation passes, it computes the centroid by averaging each dimension across all vectors. Finally, it returns the computed centroid or an error message back to the requester.

## Output Details
The workflow returns a JSON response to the original requester containing either the computed centroid or an error message if validation failed.

## Tags
vector, centroid, math, webhook, API, validation, n8n, automation, production-ready
