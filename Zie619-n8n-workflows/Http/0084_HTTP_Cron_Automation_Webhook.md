# Workflow Analysis for What To Eat

## Description
This workflow automatically finds and emails you personalized recipe suggestions based on your dietary preferences, ingredient constraints, calorie limits, and preparation time, using the Edamam recipe API.

## Input Details
The workflow is triggered daily at 10 AM via a cron schedule and uses pre-configured search criteria like preferred ingredient, diet type, health labels, calorie and time limits, along with Edamam API credentials.

## Process Summary
First, it sets user-defined search criteria such as diet, health preference, ingredient, and calorie/time limits. It then randomly selects a diet and health label if configured as 'random'. Next, it calls the Edamam API to get the total number of matching recipes. Based on that count, it picks a random subset of recipes to retrieve detailed data for. Finally, it formats these recipes into an HTML email and sends it to the user.

## Output Details
The workflow sends an HTML-formatted email containing clickable recipe links that match the user's criteria to a configured email address.

## Tags
recipe, email, cron, Edamam API, diet, health, automation, food recommendation
