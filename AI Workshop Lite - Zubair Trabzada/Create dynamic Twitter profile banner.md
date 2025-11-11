# Workflow Analysis for Twitter Follower Banner Updater

## Description
This workflow fetches the latest Twitter followers, processes their profile pictures, and updates the user's Twitter profile banner with their avatars overlaid on a background template.

## Input Details
The workflow is manually triggered by clicking 'execute' and receives no external input data.

## Process Summary
The workflow starts by fetching the last 3 Twitter followers using the Twitter API. It extracts follower data and downloads each follower's profile image, resizing and cropping them into circular avatars with a transparent background. These avatars are then overlaid onto a predefined background image at specific positions. Finally, the resulting composite image is uploaded as the user's new Twitter profile banner using OAuth1 authentication.

## Output Details
The workflow updates the user's Twitter profile banner with an image containing the avatars of their latest followers.

## Tags
twitter, social media, image processing, automation, profile banner, followers
