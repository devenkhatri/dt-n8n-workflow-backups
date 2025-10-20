# Workflow Analysis for UTM Link Generator for Analytics

## Description
This workflow generates UTM-tagged links based on predefined parameters and user input, which can be shared on platforms like LinkedIn. It helps in tracking the effectiveness of marketing campaigns.

## Input Details
The workflow is triggered manually and receives URL parameters and social media post content as input.

## Process Summary
The workflow starts by merging all the input data available. Then, it constructs a base URL for the UTM parameters. Next, it dynamically sets the UTM source and campaign based on the provided input. After that, it generates the full UTM-tagged URL and shortens it using TinyURL. Finally, it formats the output to include the shortened URL and the social media post content for easy sharing.

## Output Details
The workflow outputs a formatted text string containing the social media post content and the shortened UTM-tagged URL, ready for sharing.
