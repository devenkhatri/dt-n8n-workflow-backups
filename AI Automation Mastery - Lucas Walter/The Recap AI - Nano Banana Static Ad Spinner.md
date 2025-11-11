# Workflow Analysis for The Recap AI - Nano Banana Static Ad Spinner

## Description
This workflow automates the creation of high-converting ad variations by first analyzing a brand's website to generate comprehensive brand guidelines, then using those guidelines along with an original ad image to produce 10 strategically different ad variations that maintain the original design while testing specific elements like talent, colors, or CTAs.

## Input Details
The workflow is triggered by two separate forms: one for brand information (website URL and Google Drive folder) to generate brand guidelines, and another for ad generation (original ad image and Google Doc ID containing brand guidelines).

## Process Summary
First, the workflow scrapes the brand's website to create detailed brand guidelines stored in a Google Doc. Then, when an ad generation request is received, it combines the original ad image with the brand guidelines to create a strategic prompt for an AI. The AI generates 10 distinct ad variation instructions, which are then processed individually to create new ad images using Google's Gemini model. Each resulting ad variation is uploaded to Google Drive alongside the original source ad.

## Output Details
The workflow produces a Google Doc with brand guidelines and generates 10 ad variations that are uploaded to a specified Google Drive folder, along with the original source ad.

## Tags
ad-generation, brand-guidelines, google-drive, image-processing, ai-creative, marketing-automation, gemini-ai, google-docs
