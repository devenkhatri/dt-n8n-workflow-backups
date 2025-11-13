# Workflow Analysis for Youtube Searcher

## Description
Automated workflow to fetch and analyze Youtube video data

## Input Details
The workflow is triggered manually and receives channel IDs and URLs as input

## Process Summary
The workflow fetches video data from Youtube using the provided channel IDs, extracts relevant information such as view count, like count, and comment count, and stores it in a Postgres database. It also removes short videos, sanitizes the data, and structures it for further analysis. The workflow uses various nodes such as httpRequest, youTube, code, set, and postgres to perform these tasks.

## Output Details
The workflow produces a structured dataset of video information and stores it in a Postgres database

## Tags
automation, youtube, postgres, data analysis, video analytics
