# Workflow Analysis for Hacker News to Video Template - AlexK1919

## Description
This automated workflow processes Hacker News articles, analyzes their content for relevance to automation or AI, generates corresponding images and videos, and then prepares them for distribution. It is optimized for production use with comprehensive error handling, security, and documentation.

## Input Details
The workflow is manually triggered and fetches the latest Hacker News articles.

## Process Summary
The workflow first retrieves up to 50 Hacker News articles. For each article, it uses an AI agent to determine if the content is related to automation or AI, summarizes the article, and extracts a relevant image URL. If the article is deemed relevant, it prepares the article summary into blurbs and generates two image prompts. Then, it uses external APIs (Leonardo.ai and RunwayML) to generate two distinct images and two short videos based on the prepared prompts. Finally, it stitches these generated assets, article title, and blurbs with voiceovers into a complete video using Creatomate.

## Output Details
The workflow produces a multi-scene video for each relevant Hacker News article, incorporating AI-generated images, videos, and voiceovers.

## Tags
automation,n8n,production-ready,excellent,optimized
