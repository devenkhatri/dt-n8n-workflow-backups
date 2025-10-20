# Workflow Analysis for Paginating Data from an API

## Description
This workflow demonstrates how to retrieve all pages of data from an API that uses pagination. It handles both cursor-based and offset-based pagination strategies.

## Input Details
This workflow is triggered manually.

## Process Summary
The workflow starts by initializing variables for cursor and offset. It then calls an API in a loop, retrieving data page by page. The workflow checks for the presence of a "next_cursor" or evaluates if the "offset" has reached the "total" to determine if there are more pages. It aggregates all data from different pages into a single dataset.

## Output Details
The workflow outputs a combined dataset containing all records from the paginated API.
