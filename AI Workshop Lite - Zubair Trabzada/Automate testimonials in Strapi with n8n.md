# Workflow Analysis for Automate Testimonials in Strapi

## Description
This workflow automates the process of collecting testimonials from new database entries, proofreading them using AI, and then publishing them to Strapi.

## Input Details
The workflow is triggered by an entry created in a specified database.

## Process Summary
The workflow starts by retrieving new entries from a database. It then uses an AI model to proofread the testimonial text. After proofreading, it checks if the entry already exists in Strapi. Finally, it creates or updates the testimonial in Strapi, marking it as published if it was proofread by AI.

## Output Details
The workflow publishes or updates testimonial entries in Strapi, indicating whether they were proofread by AI.
