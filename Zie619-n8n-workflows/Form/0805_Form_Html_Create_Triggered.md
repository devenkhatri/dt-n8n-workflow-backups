# Workflow Analysis for Brightdata Workflow

## Description
This workflow allows users to select product categories and receive personalized email notifications with the latest deals from MediaMarkt, scraped and processed automatically using AI.

## Input Details
The workflow is triggered when a user submits a web form with their preferred product categories and email address.

## Process Summary
1. The workflow starts when a user completes a form selecting one or more product categories and providing their email. 2. It fetches the latest MediaMarkt offers webpage using BrightData, with location set to Spain. 3. The raw HTML content is extracted, then sent to an OpenAI model (GPT-4o-mini) to parse and generate a structured JSON list of deals filtered by the user’s selected categories. 4. The resulting deals are split into individual items and used to generate an HTML email body listing each deal with a link and price. 5. The email is sent to the user, and a confirmation message is displayed on the form completion page showing the number of deals sent.

## Output Details
The workflow sends a personalized HTML email with filtered MediaMarkt deals to the user’s provided email address and displays a success message on the form page.

## Tags
BrightData, web scraping, email automation, deal finder, form automation, OpenAI, MediaMarkt, GPT-4, e-commerce, personalized offers
