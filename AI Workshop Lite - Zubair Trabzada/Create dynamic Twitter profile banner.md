# Workflow Analysis for Automated Twitter Banner Update with New Followers

## Description
This workflow automatically fetches your latest Twitter followers, processes their profile pictures, composites them onto a predefined background image, and then updates your Twitter profile banner with the newly generated image. It helps in showcasing recent followers on your profile.

## Input Details
The workflow is triggered manually by clicking the "execute" button.

## Process Summary
First, the workflow fetches the latest three followers from Twitter. It then downloads each follower's profile image, resizes them, and crops them into a circular shape. These processed images are then further resized. Simultaneously, a template background image is fetched. Finally, the follower profile images are composited onto the background image at specific positions, creating a custom banner.

## Output Details
The workflow updates the user's Twitter profile banner with the newly generated image featuring recent followers.
