# Workflow Analysis for UTM Link Generator with Analytics

## Description
This workflow generates UTM-tagged links and tracks their performance using Google Analytics.

## Input Details
The workflow is triggered manually and takes a list of URLs and UTM parameters as input.

## Process Summary
The workflow first extracts UTM parameters and URLs from the input. It then constructs a full UTM-tagged URL for each input URL. Subsequently, it records an event in Google Analytics for each generated link, tracking the URL, campaign source, medium, and campaign name. Finally, it shortens the generated UTM links using a custom URL shortener service.

## Output Details
The workflow outputs a list of shortened, UTM-tagged URLs.
