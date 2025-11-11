# Workflow Analysis for Automated Meal Plan Generator

## Description
This workflow automatically creates a weekly dinner meal plan by selecting random recipes from a specified category in Mealie, a recipe management tool. It can run on a schedule (e.g., every Friday at 8 PM) or be triggered manually for testing.

## Input Details
The workflow is triggered either on a recurring schedule (e.g., every Friday at 8 PM) or manually via a test button, and uses predefined configuration values for recipe selection.

## Process Summary
The workflow starts by setting configuration parameters such as the number of recipes, number of days to offset the plan, and a Mealie category ID. It then fetches recipes from the Mealie API based on these settings. A custom code node randomly selects the specified number of recipes and assigns each to a future dinner date. Finally, the generated meal plan is sent to Mealie via an API POST request to create the plan in the system.

## Output Details
The workflow outputs a structured meal plan with selected recipes scheduled for upcoming dinner dates, which is sent to the Mealie application via an authenticated HTTP POST request.

## Tags
meal planning, automation, Mealie, recipe management, scheduled workflow, random selection, dinner planner
